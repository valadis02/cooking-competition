# Cooking Competition Management System

## Description
This application is a system for storing and managing information for organizing a cooking competition. It manages recipes, ingredients, and equipment required for the competition.

---

## Installation Instructions

### Prerequisites
- **MySQL**
- **MySQL Workbench 8.0 CE**
- **Visual Studio Code (VS Code)**

### Step 1: Set Up the Project in VS Code
1. Open VS Code and create a new project.
2. Copy the code from the GitHub repository into the new project.
3. Configure the database connection parameters in your code by updating the following fields:
   ```python
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
Use the code from the initialize_database.sql file to set up the database schema and relationships:
sql
Αντιγραφή κώδικα
USE db2;
-- SQL code for creating tables and inserting data
Insert Tables and Data:

Execute the SQL script files all_tables.sql and all_elements_in_tables.sql to create the necessary tables and populate them with initial data.
Set Up Queries and Triggers:

Run the SQL scripts question1.sql, question2.sql, ..., question15.sql to create the queries and triggers required by the application.
Database Structure
The database consists of several entities and relationships, including:

Recipes: Stores information about recipes, including name, description, and associated categories.
Ingredients: Manages ingredients required for recipes.
Equipment: Tracks equipment needed for cooking tasks.
Recipe Steps: Defines the sequential steps for executing a recipe.
Food Groups: Categorizes ingredients into various food groups.
National Cuisines: Groups recipes by cultural or regional origins.
Recipe Themes: Organizes recipes into thematic sections for competitions.
Chefs: Stores information about participating chefs.
Competition Episodes: Tracks individual competition rounds.
Scores: Manages scoring data for competition episodes.
Application Users: Differentiates between administrators and chefs, each with specific roles and permissions.
System Features and Roles
Administrator
Can register and modify all system data.
Has the ability to back up the database and restore it when needed.
Chef
Can manage and edit recipes assigned to them.
Can add new recipes and edit their personal information.
Does not have access to modify system-wide settings or data not assigned to them.
Functional Specifications
Recipes include a name, short description, and classification into one or more meal categories.
Recipes are tagged for categorization and may include up to 3 cooking tips.
Preparing a recipe requires specific equipment and includes preparation and cooking times.
Each recipe is composed of one or more sequential steps.
Recipes require specified quantities of ingredients grouped into food categories.
Each recipe highlights a primary ingredient that determines its classification.
Recipes may include optional nutritional information.
Competitions organize recipes into thematic sections for evaluation.
Chefs can execute multiple recipes, and each recipe can be associated with multiple chefs.
Competitions are conducted annually over 10 episodes, with structured evaluation and scoring systems.
Usage Instructions
Ensure all SQL scripts have been executed in the MySQL Workbench to initialize the database.
Run the application using Visual Studio Code.
Log in as an administrator to configure initial data or as a chef to add and manage recipes.
Authors
Tsirindanis Chrysovaladis
Email: balt5249@gmail.com
Student ID: 03120184
Sources and References
National Cuisines
Food Groups
Food Groups Institute
Calorie Meter
Chef
Recipe Database

