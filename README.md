# E-commerceBackEnd
## Description
![E-Commerce Back End](./assets/images/Screenshot%202022-05-17%20213232.png) <br/>

The E-CommerceBackEnd is a codebase, which provides the backend functionality of an E-Commerce website and allows the user to perform RESTful API CRUD (Create, Read, Update, Delete) operations on the platform. In more detail, the code in this repository provides a simple solution to setting up API endpoints to a company's Products, Categories, and Tags stored in a MySQL database. 

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Languages and Technologies Used:**

- Javascript ES6
- node.js
- MySQL
- npm (express, sequelize, mysql2, dotenv, nodemon)
- Insomnia

## Table of Contents

1. [ Installation ](#installation)
2. [ Usage ](#usage)
3. [ License ](#license)
4. [ Contributing ](#contributing)
5. [ Tests ](#tests)
6. [ Questions ](#questions)


<a name="installation"></a>

## Installation
To install the application, please follow the steps listed below: 
1. Download the latest version of node.js on your computer and ensure you have access to a MySQL account. <br/>
2. Clone this repository on your computer by opening your command-line interface and using git clone and the HTTPS or SSH URL retrieved from this repository's 'Code' dropdown above (e.g.```git clone git@github.com:TaimurHasan/E-CommerceBackEnd.git```). <br/>
3. Navigate or cd into the cloned directory from the CLI (i.e. ``` cd ./E-CommerceBackEnd ```). <br/>
4. Initialize the NPM registry, as it hosts the required packages needed to run this application, using ```npm init -y```. <br/>
5. Navigate to the '.env.EXAMPLE' file provided in this repository, edit the empty strings for 'DB_USER' and 'DB_PW' to contain your MySQL login information.
6. Rename the '.env.EXAMPLE' file to '.env' and ensure it is saved
7. Run ```mysql -u root -p``` to login into the mysql shell and run the following code line to initialize the database: ```source db/schema.sql```
8. Seed the database with provided preset seeds using ```npm run seed``` (recommended)
9. Install the required packages using 'npm i'. <br/>
10. Run ```npm start``` to initialize the server and begin testing!

<a name="usage"></a>

## Usage
To use this codebase, it is recommended to use Insomnia to test the API endpoints. See below for a list of API Endpoints available:

**GET/POST/PUT/DELETE:**
- http://localhost:3001/api/categories
- http://localhost:3001/api/categories/:id
- http://localhost:3001/api/products
- http://localhost:3001/api/products/:id
- http://localhost:3001/api/tags
- http://localhost:3001/api/tags/:id

For POST/PUT routes, please use the following object examples: <br/>
**Categories**

```
{
    "category_name": "Accessories"
}
```

**Products**
```
{
	"product_name": "Bracelet",
	"price": "12",
	"stock": "3",
	"tagIds": [7, 8],
	"category_id": "6"
}
```

**Tags**
```
{
	"tag_name": "cheap"
}
```

For more details, please refer to the [walkthrough video](https://drive.google.com/file/d/1NXRWe6K3GqqFG_hEkJVdYihOfx6Eh7EP/view).


<a name="license"></a>
## License
This project is licensed under the MIT License - see the [license info](https://opensource.org/licenses/MIT) for details.


<a name="contributing"></a>

## Contributing

This project can be contributed to by forking the application. For any contributions, please submit a Pull Request, which will be reviewed upon submission before acceptance.

<a name="tests"></a>

## Tests

This project can be tested using Insomnia (recommended) or in a browser. Please follow the steps below: <br/>
1. Navigate to the [Insomnia](https://insomnia.rest/) website and follow the download instructions (optional) <br/> 
2. Perform RESTful API operations on the endpoints listed in the 'Usage' section above <br/>

<a name="questions"></a>

## Questions

[GitHub](https://github.com/TaimurHasan) <br/>
For any questions, please send an Email to [taimurhasan11@gmail.com](mailto:taimurhasan11@gmail.com)

