Questions::
What is responsible for defining the routes of the games resource?
The file 'server/helpers/create_route.js' defines the routes.


What do you notice about the folder structure?>
The project folder structure contains a 'client' folder and a 'server' folder


Whats the client responsible for?>
The client folder contains a Vue app, for delivering the front-end of the game.


Whats the server responsible for?>
The server is responsible for receiving requests and sending responses.  The server is also configured to respond with HTTP 500 errors in the event of an internal error.


What are the the responsibilities of server.js?>
The server.js file is used to configure the server.
Using keywords such as 'require' and 'use' the server.js file configures the server to the requirements of the App. For example the Express framework, directory path and the MongoDB config.  Finally it specifies the port which it is listening on, 3000 here.


What are the responsibilities of the gamesRouter?>
The gamesRouter takes the data from the MongoDB collection and makes it available on the API endpoint.


What process does the the client (front-end) use to communicate with the server?>
The client is a Vuejs App and it uses the keyword 'fetch' to make a request to the API on localhost:3000.  It employs RESTful routes such as GET and POST to interact with the API to complete user requests.


What optional second argument does the fetch method take? And what is it used for in this application?>
The optional second argument is known as the 'init' object, this allows additional configuration of the fetch method. It can include the REST method (GET/POST etc), the mode(CORS) and header type.


Which of the games API routes does the front-end application consume (i.e. make requests to)?>
http://localhost:3000/api/games


What are we using the MongoDB Driver for?>
It provides integration between the MongoDB core and the application in which it is being used. It uses BSON which is the data storage and network transfer format used on all MongoDB documents.
