# 📚 Week 6

## 🗄️ Database Normalization

### Understanding Database Normalization
- **What is Database Normalization?**
  - Database normalization is the process of structuring a relational database to reduce data redundancy and improve data integrity.
  - It involves organizing the columns (attributes) and tables (relations) of a database to ensure that their dependencies are properly enforced.

### Normal Forms
- **1NF (First Normal Form):**
  - Each table cell should contain a single value.
  - Each record needs to be unique.

- **2NF (Second Normal Form):**
  - Be in 1NF.
  - Single Column Primary Key that does not functionally depend on any subset of candidate key relation.

- **3NF (Third Normal Form):**
  - Be in 2NF.
  - Has no transitive functional dependencies.

### 🎨 Practical Exercise: Normalizing a Database
- **Task:** Normalize the given robot inventory table to 3NF.
- **Instructions:**
  - Analyze the table and identify any data redundancy or anomalies.
  - Apply the necessary normalization steps to achieve 1NF, 2NF, and 3NF.
  - Create the normalized tables and define the primary and foreign key relationships.

### 💡 Discussion
- Discuss the benefits of database normalization in terms of data integrity, storage efficiency, and maintainability.
- Explore the trade-offs between normalization and performance in real-world scenarios.

## 📋 SQL CREATE TABLE

### Understanding CREATE TABLE
- **What is CREATE TABLE?**
  - The CREATE TABLE statement is used to create a new table in a database.
  - It defines the structure of the table, including the column names, data types, and constraints.

### Basic Syntax of CREATE TABLE
- **Syntax:**
  ```sql
  CREATE TABLE table_name (
      column1 datatype,
      column2 datatype,
      column3 datatype,
      ...
  );
  ```

- **Example:**
  ```sql
  CREATE TABLE robots (
      id INT PRIMARY KEY,
      name VARCHAR(255),
      model VARCHAR(100),
      manufacturer VARCHAR(255)
  );
  ```

### 🌍 Practical Exercise: Creating Tables for a Robot Database
- **Task:** Create tables for a robot database using SQL CREATE TABLE statements.
- **Instructions:**
  - Design tables for robots, components, and assembly records.
  - Define the appropriate columns, data types, and constraints for each table.
  - Establish primary and foreign key relationships between the tables.
  - Execute the CREATE TABLE statements to create the tables in the database.

### 💡 Discussion
- Discuss the importance of choosing appropriate data types and constraints when creating tables.
- Explore best practices for naming tables and columns in a database.

## 🔑 Primary Key and Foreign Key

### Understanding Primary Key
- **What is a Primary Key?**
  - A primary key is a column or set of columns that uniquely identifies each record in a table.
  - It ensures the integrity and uniqueness of the data within the table.

### Understanding Foreign Key
- **What is a Foreign Key?**
  - A foreign key is a column or set of columns in one table that refers to the primary key of another table.
  - It establishes a link between the data in two tables and enforces referential integrity.

### 🎨 Practical Exercise: Implementing Primary and Foreign Keys
- **Task:** Modify the tables created in the previous exercise to include primary and foreign keys.
- **Instructions:**
  - Identify the appropriate columns to serve as primary keys for each table.
  - Alter the table definitions to add primary key constraints.
  - Establish foreign key relationships between the tables based on the identified relationships.
  - Update the CREATE TABLE statements to include the primary and foreign key constraints.

### 💡 Discussion
- Discuss the role of primary and foreign keys in maintaining data integrity and establishing relationships between tables.
- Explore the concept of referential integrity and its importance in database design.

## 📊 Data Definition Language (DDL)

### Understanding DDL
- **What is DDL?**
  - DDL stands for Data Definition Language.
  - It is a subset of SQL used to define and manage the structure of database objects.
  - DDL statements are used to create, modify, and delete database objects such as tables, indexes, and constraints.

### Common DDL Statements
- **CREATE:**
  - Used to create new database objects, such as tables, views, or indexes.
  - Example: `CREATE TABLE robots (...);`

- **ALTER:**
  - Used to modify the structure of existing database objects.
  - Example: `ALTER TABLE robots ADD COLUMN serial_number VARCHAR(20);`

- **DROP:**
  - Used to remove database objects from the database.
  - Example: `DROP TABLE robots;`

### 🧩 Practical Project: Robot Inventory System

### Project Description
- Develop a simple robot inventory system using SQL and the concepts learned in Week 6.
- The system should allow managers to track robot models, components, and assembly records.

### Project Requirements
- Design and create tables for robots, components, and assembly records using SQL CREATE TABLE statements.
- Normalize the database to 3NF to ensure data integrity and minimize redundancy.
- Implement primary and foreign key constraints to establish relationships between tables.
- Use DDL statements to create, modify, and delete database objects as needed.

### 🚀 Implementation Steps
- Step 1: Analyze the requirements and design the database schema for the robot inventory system.
- Step 2: Write SQL CREATE TABLE statements to create the necessary tables with appropriate columns and data types.
- Step 3: Apply normalization techniques to the tables to achieve 3NF.
- Step 4: Identify and implement primary and foreign key constraints to establish relationships between tables.
- Step 5: Use DDL statements to make any necessary modifications to the database structure.
- Step 6: Test the database by inserting sample data and verifying the integrity and relationships.

### 💡 Discussion
- Discuss how the concepts learned in Week 6 (Database Normalization, CREATE TABLE, Primary Key, Foreign Key, DDL) are applied in the robot inventory system project.
