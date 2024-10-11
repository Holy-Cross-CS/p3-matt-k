CSCI 356 Fall 2024 Project 3 Starter Code
-----------------------------------------

This repository contains starter code for project 3, in which you will implement
the whisper web app. 

* `web_files` - The files implmenting the client half of the whisper app.

Tasks:

- [x] implement the client half of the whisper app
- [x] add webserver.py for the server half, borrowing from earlier project
   - [x] print the appropriate URL for whisper app to console
- [x] handle GET for topic list
   - [x] handle version 0 as a temporary stop-gap
   - [x] handle version 1 as a temporary stop-gap
   - [x] handle any version N, the general case, with proper wait/notify\_all
   - [x] return appropriate errors if topic not found or other errors
- [x] handle POST for messages
   - [x] return appropriate errors if request is malformed or other errors
- [x] handle GET for topic message feed
   - [x] handle any version N, with proper wait/notify\_all
   - [x] return appropriate errors if topic is not found or other errors
- [x] handle POST for liking a topic
   - [x] return appropriate errors if topic is not found or other errors
- [ ] reach goal: topics are sorted by some criteria
- [ ] reach goal: limit each topic to only the most recent messages
- [ ] reach goal: implement downvoting/removal of messages
- [ ] reach goal: implement other features, e.g. using cookies, etc.
- [ ] project still does not use HTTP related python libraries or modules
- [ ] does not crash under normal usage
- [x] Update README.md to describe final state of project, collaboration, etc.


My POST function is not incrementing correctly, as when I start the game, topics list is 0 as it should be. I click like, and topics list stays at zero, when it should be incrementing to 1, and message list version correcly increments to 1. When I click like again, topics list correctly increments to 2, which allows two likes to display on the screen, but message list does not increment and stays at 1. When I click like again (now the third time), topics list stays at 2 when it should be 3, and message list correctly increments to 3.