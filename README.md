# mini-pastebin

[A project for LiftLabs]

A small clone of pastebin [Node.js + ES6 + MongoDB]

Link: https://mini-pastebin.herokuapp.com (deployed to Heroku)

Testable with curl and Postman

This is a RESTful API that supports the following operations:

- GET /paste/:author
  - Get all pastes by author name
  - e.g. https://mini-pastebin.herokuapp.com/paste/zachary
- POST /paste/:author
  - Create a new paste with author name
  - The POST request should include a body with the following format:
    - title: [String]
    - body: [String]
    - author: [String]
    - syntax: [String] // e.g. C++, Java, etc.
- DETELE /paste/:id
  - Delete a paste by its unique id
- PATCH /paste/:id
  - Modify a paste by its unique id
  
Extra feature ("easter egg"):

- GET /git-pun
  - Get a random git joke (they are all terrible)
