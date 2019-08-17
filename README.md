# Which Sandwhich? :fork_and_knife:

 https://fast-fortress-18955.herokuapp.com/

## Overview

Restaurant app that lets users input the names of the sandwich they'd like to eat.

## Functionality Breakdown
This **full-stack site** deployed on Heroku takes in and stores sandwhiches from the user then allows them to either eat the sandwich, delete the sandwich or remake it to eat again. 

## Technology Used
- MySQL
- Node
- Express
- Handlebars
- ORM and MVC design pattern
- JavaScript
- JQuery
- Boostrap
- HTML

## Technical Approach
Orgnaize the directories to be as below:
 .
├── config
│   ├── connection.js
│   └── orm.js
├── controllers
│   └── sandwhich_controller.js
├── db
│   ├── schema.sql
│   └── seeds.sql
├── models
│   └──sandwhich.js
├── node_modules
├── package.json
├── public
│   └── assets
│       ├── css
│         └── sandwich_style.css
├── server.js
└── views
    ├── index.handlebars
    └── layouts
        └── main.handlebars


1. Install npms to be required - express, express-handlebars, mysql, dotenv
####DB Setup
1. Set up the schema.sql file with the sandwich database and sandwiches table
1. Set up seeds.sql file with insert queries to populate the sandwiches table
1. Run schema.sql and seeds.sql files to create the database
1. Inside the connection.js file, setup the code to connect Node to MySQL.Export the connection
1. Create an orm.js file with the following:
    1. require connection.js
    1. Methods that will execute the necessary MySQL commands in the controllers. These are the methods that will be used in order to retrieve and store data in the database.
       selectAll()
       insertOne()
       updateOne()
  - Export the ORM object in module.exports.
  
1. Set up the burger.js file the models folder with the following:
    1. Import orm.js into burger.js
    2. Code that will call the ORM functions using burger specific input for the ORM.
    3. Export the burger.js file.
1. 
