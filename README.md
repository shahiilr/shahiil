# URK23CS5097

Food Order System (Java + MySQL)
This project is a Java GUI-based Food Ordering System that allows users to:

Register an account
Log in to their account
Select food items from a menu
Enter delivery details (Name, Mobile No, Location)
Submit and store their orders in a MySQL database

Rate their order experience

The system is built using Java Swing for the GUI and MySQL for backend database storage.

Features
User Registration and Login system

Food Menu display with item selection

Quantity control with "+" and "–" buttons

Automatic calculation of total price

Form submission capturing:

Name

Mobile Number

Food Items

Total Price

Delivery Location

Rating

Database connection using JDBC

User-friendly GUI interface

Database Structure (MySQL)
Table: orders


Column Name	Data Type	Description
id	INT (Auto Increment)	Unique Order ID
name	VARCHAR(255)	Customer Name
mobile_no	VARCHAR(15)	Customer Mobile Number
food_item	VARCHAR(500)	Selected Food Items
total_price	DECIMAL(10,2)	Total Order Price
location	VARCHAR(255)	Delivery Location
rating	INT	Customer Rating (1-5 Stars)
Java Files Overview

File Name	Description
DBConnection.java	Handles database connection setup (MySQL)
RegisterPage.java	GUI for new user registration
LoginPage.java	GUI for existing user login
WelcomePage.java	Welcome page after successful login
MenuPage.java	GUI for menu selection and order submission
How to Run the Project
Set up MySQL Database:

Create a new database (e.g., food_order_system).

Create the orders table using the above structure.

Update Database Configuration:

In DBConnection.java, update your database URL, username, and password if needed:

java
Copy
Edit
String url = "jdbc:mysql://localhost:3306/food_order_system";
String user = "root";
String password = "your_password";
Compile Java Files: If you have .java files:

bash
Copy
Edit
javac DBConnection.java LoginPage.java RegisterPage.java WelcomePage.java MenuPage.java
If you only have .class files, you can directly run them.

Run the Application:

Start with LoginPage.java or RegisterPage.java.

bash
Copy
Edit
java LoginPage
or

bash
Copy
Edit
java RegisterPage
Requirements
Java JDK 8 or higher

MySQL Server

MySQL JDBC Driver (Connector/J)


Screenshots:

![image](https://github.com/user-attachments/assets/2cb6afb6-51dd-41f1-b595-c7228349a91d)

![image](https://github.com/user-attachments/assets/be24c537-9a5c-4fe5-8673-946720539f8f)

![image](https://github.com/user-attachments/assets/401531fa-d961-46d3-bac0-48d11d94d846)

![Uploading image.png…]()





