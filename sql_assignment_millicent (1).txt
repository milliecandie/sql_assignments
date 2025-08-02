# Step 1:Create the salesDB Database

CREATE DATABASE salesDB;

# Step 2:Use the salesDB Database

USE salesDB;

# Step 3:Create a Table Called Customers

CREATE TABLE Customers (
  CustomerID INT PRIMARY KEY,
  FirstName VARCHAR(50),
  LastName VARCHAR(50),
  Email VARCHAR(100),
  Phone VARCHAR(20),
  City VARCHAR(50)
);

Step 4:Insert Some Samples Records

INSERT INTO Customers (CustomerID, FirstName, LastName, Email, Phone, City)
VALUES
(1, 'Millicent', 'Makokha', 'millie@gmail.com', '0700000001', 'Nairobi'),
(2, 'Brian', 'Otieno', 'brian@gmail.com', '0700000002', 'Kisumu'),
(3, 'Grace', 'Chebet', 'grace@gmail.com', '0700000003', 'Eldoret');

Step 5:Select all Data from the Table 

SELECT * FROM Customers;

Optional Step:Filter by City

SELECT * FROM Customers
WHERE City = 'Nairobi';