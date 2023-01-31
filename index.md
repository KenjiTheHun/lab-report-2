# Lab Report 2 - Servers and Bugs (Week 3)
## Part 1 - String Server
For this part, I based my implementation of String Server on the NumberServer.java provided during the lab:

![Image](SearchLines.png)

I tested out my code by opening a local server on port 4000 and added two strings:

![Image](add1.png)

- Which methods in your code are called?

The handleRequest method is called upon entering the local server

- What are the relevant arguments to those methods, and the values of any relevant fields of the class?

`searches` is the ArrayList containing all added messages. 
`url` is the url input, typically entered as `localhost:(port number)/add-message?=(message)`. 
`parameters` is the the array of strings containing the url split up on `=`. 
`result` is the collection of all added messages used to display the messages

- How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

`url` becomes `localhost:4000/add-message?s=hello`.
`parameters` becomes `localhost:4000/add-message?s` and `hello`.
`searches` becomes `hello`.
`result` becomes `hello`.
`element` becomes `hello`.


