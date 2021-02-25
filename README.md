# Play Backend 

This repo acts as a play backend for you to familiarize yourself with different API endpoints. The routes below outline the different endpoints you can hit. 


### Set Up Instructions 
1. fork and or clone this repository. 
2. cd into the repo and then cd into the backend folder. 
3. run `npm install`
4. Make sure you have Postgres running. 
5. run `psql -f db/schema.sql`
6. run `node app.js`

Users have the following properties:
 * id INTEGER (don't include this on post requests)
 * username TEXT

 Cars have the following properties: 
*  id INTEGER (don't include this on post requests)
* brand TEX 
* model TEXT
* year INTEGER
* owner_id points to a users id. 

All routes can need to start with `http://localhost:3000`

* /cars - get all cars GET

* /cars/:id - get single car GET

* /cars - create car POST

* /cars/:id - delete car DELETE

* /cars/:id - update car PUT

* /cars/:id - update only a specific car feature PATCH

* /users - get all users GET

* /users/:id - get single user GET

* /users/:id - delete single user DELETE

* /users - create user POST

* /users/:id/cars - get all cars for a specific user GET