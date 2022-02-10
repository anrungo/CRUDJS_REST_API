## Pacotes instalados
npm init
npm install express
npm install mongodb
npm install mongoose
npm install -g nodemon --save-dev

## Edit on scripts:

`"scripts": {
    "start": "nodemon app.js"
  }`

vamos usar o URL local:
 - GET : http://localhost:8080/aliens
 - GET : http://localhost:8080/aliens/<id>
 - POST : http://localhost:8080/aliens 
 - PATCH : http://localhost:8080/aliens/<id>

 - GET : http://localhost:8080/books

A serem testados usando o postman.

To run the code we need to use: `nodemon run start`

And we have:
`[nodemon] 2.0.15
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: js,mjs,json  
[nodemon] starting `node run start app.js`  
connected...`

We have the concept of MVC (Model, View, Controller)

M - Model       - SCHEMA ==> Database object
V - View        - UI     ==> Every website should have good view
C - Controller  - Router ==> Controls all the routing

Different entities should have different models.

RDBMS     -   MONGODB
Database  -   Database
Tables    -   Collections
Rows      -   Documents
Columns   -   Fields

To send data we need to use a post request: router.post().
From postman we use POST: in postman on Body.
{
  "name": "Navin",
  "tech":"NodeJS"
}
