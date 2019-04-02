# Lab-Authentication

### Author: Gregory Dukes   with AaronF, Cory, Jon, Vanessa, Alex, Spencer

### Links and Resources
* [repo](https://github.com/dukes-js-401/Lab-Authentication/pull/1)
* [travis](http://xyz.com) badge coming soon
* [heroku](https://strawberry-cupcake-28495.herokuapp.com/) 

#### Documentation
* [swagger](http://xyz.com) (API assignments only)
* [jsdoc](http://xyz.com) (All assignments)

### Modules
-/auth
- middleware.js
  * handles the business logic for user authentication
- router.js
  * handles the post routes from the app.js
- users-model.js
  * handles the user models and querying the db

-/middleware
- 404.js
- error.js

-/routes
- book.js


### Setup
#### `.env` requirements
* `PORT` - :3000
* `MONGODB_URI` - URL to the running mongo instance/db

#### Running the app
* `npm start`
* Endpoint: `echo '{"username":"<name>", "password":"<password>"}' | http post :3000/signup`
  * Returns a JSON object with a user token.
* Endpoint: `http post :3000/signin -a greg:password123`
  * Returns a JSON object with a user token.
* Endpoint: `http :3000/books`
  * Returns an error, "Invalid Username or Password"
* Endpoint: `http :3000/books -a <username>:<password>`
  * Returns a JSON object with all books from db.

#### Tests

#### UML
Link to an image of the UML for your application and response to events
