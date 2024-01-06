# e-commerce-back-end-with-sequelize

---

## Table of Contents

- [Project Description](#project-description)
- [How to run this project](#how-to-run-this-project)
- [How to use this project](#how-to-use-this-project)
- [Credits](#credits)
- [License](#license)

## Project Description

This project is a back end demo for an e-commerce website that utilizes CRUD operations to modify table data and manage the associations between them.

## How to run this project

Click on the following image to view the demo video:
<!-- Change title / image / video info -->
[![MySQL DB Employee Tracker - demo](<assets/images/MySQL DB Employee Tracker - demo.png>)](https://drive.google.com/file/d/1_KThXrsfNdhVv8Z1D5NXUuXRIdfuJCvh/view)

Make sure Node.js is installed on your device. You can open the command terminal and enter "node -v" to check if node is installed. If the command terminal responds back with a version of Node, then it is installed. Otherwise, go to https://nodejs.org/en/download/ and download the LTS version of Node for the appropriate OS that you are using (Windows, Mac, Linux, etc.).

Open the command terminal (if you haven't already done so). Enter "node server.js" to initiate the program.

## How to use this project

After initiating the program, you can open a browser and navigate through the database from localhost:3001 via GET requests. Additional software is necessary to utilize POST, UPDATE, and DELETE requests.

This back end was tested with Insomnia REST API, which can be downloaded from here:

https://insomnia.rest/download

### READ all info from a table

Get all data from a table using any of the following routes:

- localhost:3001/api/category
- localhost:3001/api/product
- localhost:3001/api/tag

### READ info about one instance from a table

Get all data from one instance of a table using any of the following routes:

- localhost:3001/api/category/:id
- localhost:3001/api/product/:id
- localhost:3001/api/tag/:id

Replace :id with the ID of the requested instance.

### CREATE a new instance for a table

Post an instance for a table using any of the following routes:

- localhost:3001/api/category
- localhost:3001/api/product
- localhost:3001/api/tag

The POST request body should look something like this:

{
  product_name: "Basketball",
  price: 200.00,
  stock: 3,
  tagIds: [1, 2, 3, 4]
}

### UPDATE an instance from a table

Modify (put) an instance in a table using any of the following routes:

- localhost:3001/api/category/:id
- localhost:3001/api/product/:id
- localhost:3001/api/tag/:id

Replace :id with the ID for the instance that you are modifying.

The PUT request body should look something like this:

{
  product_name: "Basketball",
  price: 200.00,
  stock: 3,
  tagIds: [1, 2, 3, 4]
}

### DELETE an instance from a table

Remove an instance from a table using any of the following routes:

- localhost:3001/api/category/:id
- localhost:3001/api/product/:id
- localhost:3001/api/tag/:id

Replace :id with the ID for the instance that you are removing.

## Credits

Tyler Odo

## License

Default
