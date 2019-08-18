# MessageApp Kata

This is a kata where you are going to implement a simple version of a messaging app, without the need to send any other thing besides text. 

there are two ways of working this kata:

- High level architecture overview
- Code Implementation

## First iteration

In this first iteration you need to design the api that you application will talk to. The application can:

- Create a user
- Add a contact
- List contacts
- Send a message to a contact

The main requirements to implement the API are:

- The messages should always be in the right order even if you have problems in your network and they are received in a different order than the one that was sent.
- You should have an REST api that respects the proper status codes and naming conventions

## Second Iteration

In this second iteration you need to implement a way to store the messages, you have to assume that you are expecting a large number of messages, so you have to use your data store in a very optimised way.

- You should store the messages in a persistent data store
- The database should be properly indexed
- Must be able to retrieve the messages using a endpoint

## Third Iteration

Now you need to filter the messages by timestamp

- The starting timestamp should be sent in the endpoint
- The filtering for the should be done at database level

## Fourth Iteration

Since the application is receiving a large number of messages we are going to implement a caching mechanism in front of the database. 

- You should use a in-memory caching without using third party tools
- It should handle millions of messages

## Fifth Iteration

This is the last iteration is to implement the functionality of a group chat.
