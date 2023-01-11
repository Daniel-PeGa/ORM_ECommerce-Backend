# ORM_ECommerce-Backend

This project is structured with MySQL. It's a simple app's backend for ecommerce that allows you to search for a product based on its category, tag, or just the product itself. It allows to find, to add, and to delete them. It works only on desktop, but its pretty cool.

## Project Description

This is the backend of an ecommerce site that is configured to use Sequelize to interact with MySQL dadtabase. It allows for adding items, categories, and tags, as well as searching for them, or deleting them. 

## Technologies Used

* Node.js
* Express.js
* Sequelize
* MySQL
* dotenv

## Install and Run

The app can't really be deployed because it's just the backend lol, but it's pretty simple to use. All you have to do is clone the github repository and open it on your code editor. Make sure to add a .env file with the following info on it:

```
DB_NAME='ecommerce_db'
DB_USER='root'
DB_PASSWORD=''
```

Once you've created the file, you can go ahead and open the integrated terminal and type in the following commands:

```
npm i
mysql -uroot -p
```

And you type in your password for mysql if you have one. Otherwise you can skip the -p in the command line. Once you are in the MySQL, type in the following commands:

```
source db/schema.sql
quit
npm run seed
node server.js
```
Then, open Insomnia or ThunderClient and go at it!

## User Story

AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

## Acceptance Criteria

GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database

## Screenshot

<img width="1470" alt="Screenshot 2023-01-11 at 2 29 34 PM" src="https://user-images.githubusercontent.com/106125888/211911250-863181cb-7e31-4f00-8860-6e02b7d85fd8.png">

