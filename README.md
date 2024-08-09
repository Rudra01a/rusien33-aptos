# rusien33-aptos
The Objective of the Program
The purpose of this module is to allow users to send customized messages on the blockchain, linked to their account address. The stored message can be updated if it already exists. This is done with a Message struct, which is pushed to the blockchain and whose owner can be changed.

The main features
Message Structure:

The message struct is the central data structure in this module. It has one field called my_msg, which stores string messages.
message_fun Function: .

This is the main function of the module. It allows the user to create a new Message struct and store it on-chain if it does not already exist. If the message already exists, this function updates the existing message with the new value.
Testing tasks:

The test_message function creates a test case that creates and updates a message for a test account. Make sure the message is properly updated with the expected return.
How does it work?
When the user calls the message_fun function, the module checks if the Message struct already exists for the user's account.
Otherwise, the function creates a new Message struct with the given message and stores it in the chain.
If so, the process updates the existing Message with the new message.
The test_message function performs an automated test to ensure that the message_fun function behaves correctly. It creates the account, saves the message, updates it, and checks if the final message looks as expected.
Take the Use of Information
This module can be used in situations where users need to store and manage simple chain messages or data points associated with their accounts. The Move programming language in the Aptos blockchain is a prime example of how on-chain data storage and updating works.
