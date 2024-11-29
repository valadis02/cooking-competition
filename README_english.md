Cooking Competition Management System
Description
This application is a system for storing and managing information for organizing a cooking competition. It manages recipes, ingredients, and equipment required for the competition.

Installation Instructions
Prerequisites
MySQL
MySQL Workbench 8.0 CE
Visual Studio Code (VS Code)
Step 1: Set Up the Project in VS Code
Open VS Code and create a new project.
Copy the code from the GitHub repository into the new project.
Configure the database connection parameters in your code by updating the following fields:
python
Αντιγραφή κώδικα
host="localhost"
user="root"
password="12345"
database="db2"
Step 2: Create the Database in MySQL Workbench
Launch MySQL Workbench:
Open MySQL Workbench from the start menu or desktop icon.
Connect to the MySQL Server:
On the home screen of MySQL Workbench, select an existing connection or create a new one if not available.
Click the Connect button to access the server.
Create the Database:
Open the SQL Editor and run the following command to create the database:
sql
Αντιγραφή κώδικα
CREATE DATABASE db2;
Use the code from the initialize_database.sql file to set up the database and tables:
sql
Αντιγραφή κώδικα
USE db2;
-- SQL code for creating tables and inserting data
Create Tables and Insert Data:
Execute the code from all_tables.sql and all_elements_in_tables.sql to create the necessary tables and insert data.
Create Queries and Triggers:
Run the code from question1.sql, question2.sql, ..., question15.sql to set up the required queries and triggers.
Database Structure
The database consists of the following entities:

Recipes
Ingredients
Equipment
Recipe Steps
Food Groups
National Cuisines
Recipe Themes
Chefs
Competition Episodes
Scores
Application Users
Roles in the System
Administrator
Registers and modifies all necessary data.
Can create a backup of the entire database and restore the system from it.
Chef
Edits all recipe-related data assigned to them and can add new recipes.
Manages their personal details.
Cannot modify other system data.
System Specifications and Assumptions
Each recipe has a name, a short description, and belongs to one or more meal categories.
Recipes are categorized via tags and can have up to 3 practical tips.
Preparing a recipe requires specific equipment and preparation/cooking time.
Each recipe consists of one or more steps to be executed sequentially.
Recipes require specific ingredients in quantities, grouped into food categories.
Each recipe has a primary ingredient that defines its category.
Recipes may include nutritional information.
The competition organizes recipes into thematic sections.
Each recipe can have one or more chefs who can execute it.
The competition occurs annually in 10 episodes/iterations with specific selection and scoring processes.
Authors
Tsirindanis Chrysovaladis
Email: balt5249@gmail.com
Student ID: 03120184
Sources
National Cuisines
Food Groups
Food Groups Institute
Calorie Meter
Chef
Recipe Database
