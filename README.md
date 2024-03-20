# E-Commerce Back End [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/blog/license/mit-0)

## Description

Welcome to E-commerce Back End!

This application is set to provide an interactive database, to help users utilize the latest technology in the e-commerce world. 

## Table of Contents
  - [Description](#description)
  - [License](#license)
  - [Installation](#installation)
  - [Tests](#tests)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [Questions](#questions)

  ## License 

  E-Commerce Back End is under MIT Licensing.<br />
  Click the license badge above for more information regarding this license.

  ## Installation
  Required items to run application: Node Package Manager, MySQL account, and an API testing platform (Insomnia or Postman will work).<br/>
  To install the application, before running enter this code block text in the integrated terminal after installing.

    npm i

  ## Tests 
To run the application,

Step: 1. <br />
Right click on db folder, and enter the Integrated Terminal. Then enter the code below for MySQL login information.

    mysql -r (username) -p

*Enter password for MySQL*<br />

Step: 2. <br />
Right click on seeds folder, and enter the Integrated Terminal. Then enter the code below to run seeds

    npm run seeds

Step: 3. <br />
Right click on server.js file, and enter the Integrated Terminal. Then enter the code below to run server

    npm start

  ## Usage

Once the the E-commerce Back End is initiated, open your choice of API testing platform, and enter the URL for the localhost and api as the parameter for the data: http://localhost:3001/api/

From here, there will be 3 sections the user can pull and manipulate data from:
1. Categories http://localhost:3001/api/categories
2. Products   http://localhost:3001/api/products
3. Tags       http://localhost:3001/api/tags

In each one of these sections, HTTP requests such as GET, POST, PUT, and DELETE will provide the user to receive, create, and delete data from the database that houses the sections. 

GET Requests: 
In order to execute GET requests (from Categories, Products or Tags), the user just needs to enter one of the three urls provided above and send the request to retreive the data information.

POST Requests: 
In order to execute POST requests (to Categories, Products or Tags), the user just needs to enter one of the three urls provided above, and then enter a body (in json format) to include the new information before sending the request. The json body structure to POST for each section shows below: 

Categories Body:<br/>

    {
        "category_name": "*STRING*"
    }

Products Body:<br/>

    {
    "product_name": "*STRING*",
    "price": *DECIMAL*,
    "stock": *INTEGER*,
    "tag_id" *[INTEGER]*: 
    }

Tags Body:<br/>

    {
        "tag_name": "*STRING*"
    }

PUT Requests: 
In order to execute PUT requests (to Categories, Products or Tags), the user just needs to enter one of the three urls provided above, AS WELL AS, where the user wants the change (PUT) to exist. To delcare where, the user must specifiy the last parameter in the URL to match the id of the data they want to change. <br />
Example URL for PUT request: <br />
http://localhost:3001/api/categories/3<br />
The last parameter of '3' is the identity of the data the user is wanting to change. <br />
After identifying what the PUT request will alter, we can follow the exact same steps in POST, where we enter the correct json format for that selected section. 

DELETE Requests: 
In order to execute DELETE requests (to Categories, Products or Tags), the user just needs to enter one of the three urls provided above, AS WELL AS, where the user wants the delete to exist. To delcare where, the user must specifiy the last parameter in the URL to match the id of the data they want to change. <br />
Example URL for DELETE request: <br />
http://localhost:3001/api/tags/3<br />
The last parameter of '3' is the identity of the data the user is wanting to delete.


[Here's a link to the Walkthrough Video!](https://drive.google.com/file/d/1KNW_j5VY1aaXQE73g3WTlYDC-z2yRbw1/view)

![Screenshot1](/lib/images/Screenshot%202024-03-20%20at%202.15.39 PM.png)
![Screenshot2](/lib/images/Screenshot%202024-03-20%20at%202.15.58 PM.png)


Woah, a Congratulations are in order. "CONGRATULATIONS", on using the best "whelming" piece of software that was ever made for the UNIVERSE! "Yahoooo!"

  ## Contributing 

  KU BootCamp

  ## Questions
  Application questions? 
  
  GitHub Account: [emmatar](https://github.com/emmatar)

  Have More Questions?!

  Email me here: m.matar515@gmail.com
  

  
