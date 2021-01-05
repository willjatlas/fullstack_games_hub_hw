Homework - Full Stack Games Hub App.

Task - (.png in this folder)

Questions
1. What is responsible for defining the routes of the games resource?
A.The server is resposible, in this case, "helpers/create_router.js".

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?
A. Each layer of the full stack is kept clean and seperate from one another in the file structure. The client contains the front end (react) scripts, and the server contains our back end scripts (express server and mongodb database).

3. What are the the responsibilities of server.js?
A. Server.js connects to our mongodb and utalizes express to act as a server that listens on the directed port. It and also handles routing, importing them from the create_router file in helpers. 

4. What are the responsibilities of the gamesRouter?
A. The gamesRouter is an instance of our create_router that handles the routing requests made to the server.

5. What process does the the client (front-end) use to communicate with the server?
A. The front end uses react's fetch methods, using the specified url. 

6. What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs
A. The second argument allows us to pass an object containing custom settings . In this case, we are using it to specify that this request is a post, and we are passing a jsonified version of our payload (user's form input).

7. Which of the games API routes does the front-end application consume (i.e. make requests to)?
A. Get, post, and delete. 

8. What are we using the MongoDB Driver for?
A. The driver allows node applications to connect to the database and work with the data. 

Extension
10. Why do we need to use ObjectId from the MongoDB driver?
A. The database defines each object inputted by genereating it's own unique id. To be able to access a particular object, we want to be able to match id in our routes. 

11. Add to your diagram the dataflow for removing a game.
(.png in this folder)