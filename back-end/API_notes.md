# Why do we need APIs?

It's like a contract between the data provider and the data user/developer. It tells the data user how they can interact with data and things that are allowed. These are the objects, methods and protocols that you can use to access them. And we won't change these things without notifiying you

A more refined definition:

> An Application Programming Interface(API) is a set of commands, functions, protocols and objects that programmers can use to create software or interact with an external system.

Putting into practice -->

When preparing to use an API there are 4 things to keep in mind:

    - Endpoint
        - Every API that interacts with an external system like a server will have an endpoint
        - They will always tell you want it is in the documentation

    - Paths
        - Narrow down on a specific piece of data that you want from the server
        - have to specifiy a specific path after the endpoint i.e the root directory
        - /Programming

    - Parameters
        - a custom query
        - parameters go at the end of the URL after the ?
        - ?contains=thequeryword
        - if we have more than one query its followed by &
        - /Programming?contains=debugging&type=single
        - the order in which you put the parameters doesn't matter

    - Authentication
        - Every time you make a request through the API they have to be able to keep track of how often you are accessing there data to determine how to charge you and monitize their data
        - Autenticated API with key

    # Authentication & Postman

    Often times when were testing API i.e trying different queries we will use a tool called __Postman__
