# Destin-Trang-P1
## Description
The following project is a mock project for a client, where I designed and developed a database for managing the distribution and tracking of products for the client. The database will control the flow of products starting from when it's manufactured at a production house to when it's purchased at a store, and record timestamps of the product's journey. It also allows for tracking of individual product history, and returning faulty products back to the production house. 

## Features
* Used SQL Server Management Studio to design an ER diagram and database.
* Used T-SQL queries to generate useful product information, such as product and order history.
* Created a tracking system that records when a product reaches certain points in its production line.
* Allows customers to purchased products from a physical store, and also sell that product back, sending it back to the production house it was manufactured at.

## Getting Started
* Download the project files from this repository.
* Using SQL Server Management Studio, restore the database using the .bak file given in the files.

## Usage
* "exec PurchaseProduct productID, storeID, productType": Stored procedure that simulates a specific client purchasing a product at a given store.
* "exec ReturnProduct productID, customerID, storeID": Stored procedure that simulates a customer returning a product to the same store that they bought the product from.
* "exec ViewPurchases": Stored procedure that displays all the purchase made so far amongst all customers.
* "exec ViewProductHistory productID": Stored procedure that displays a given product's location and transaction history.
* "exec RequestProduct storeID, productType": Stored procedure that simulates a store requesting a certain product from its assigned production house.