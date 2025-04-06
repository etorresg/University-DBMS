# University Database Management System (DBMS)
## Project Overview
This project showcases a Database Management System (DBMS) developed for managing university-related data. The system includes multiple tables to store information about students, courses, instructors, and enrollments. The database is structured to allow querying, updating, and maintaining relationships between the entities, ensuring data integrity and consistency.

Key Features:
Tables for Students, Courses, Instructors, and Enrollments

Dummy Data included for testing purposes

ERD Diagram to visualize the relationships between entities

SQL Scripts for table creation and data insertion

Project Files
1. ERD Diagram
The Entity-Relationship Diagram (ERD) provides a visual representation of the database structure, showing how tables are related to each other.

File: university_erd.png

Description: Visual diagram of the database schema, detailing entities and their relationships.


2. VDSX File
File: university_schema.vdsx

Description: This file contains the visual schema of the database, which can be opened using Visio or any other VSDX file viewer.

3. SQL Scripts
The following SQL scripts are used to create the database schema and populate it with dummy data for testing purposes:

File: create_tables.sql

Contains SQL statements to create all necessary tables.

Defines primary keys, foreign keys, and other constraints.

File: insert_dummy_data.sql

Contains SQL INSERT statements to populate the tables with sample data.

Setup Instructions
Prerequisites
Database Server: Make sure you have access to a SQL-compatible database (e.g., MySQL, PostgreSQL).

SQL Client: You can use any SQL client to run the scripts (e.g., MySQL Workbench, pgAdmin, or command-line tools).

Steps to Set Up
Create the Database:
Use the following SQL command to create a new database:

sql
Copy
Edit
CREATE DATABASE university;
Run the SQL Scripts:

First, execute create_tables.sql to set up the database schema:

sql
Copy
Edit
SOURCE create_tables.sql;
Then, execute insert_dummy_data.sql to populate the tables with test data:

sql
Copy
Edit
SOURCE insert_dummy_data.sql;
Verify the Data:
After executing the scripts, you can query the tables to ensure the data has been populated correctly:

sql
Copy
Edit
SELECT * FROM students;
SELECT * FROM courses;
SELECT * FROM instructors;
View the ERD:
Open the university_erd.png image to see a diagram of the database structure and relationships between entities.

Project Details
Tables:

Students: Stores information about students including their name, major, and enrollment status.

Courses: Contains course details such as course name, code, and credits.

Instructors: Holds instructor details, including name, department, and contact info.

Enrollments: Represents the relationship between students and courses, with a grade column.

Relationships:

A student can be enrolled in multiple courses.

A course can have multiple instructors teaching it.

Enrollments link students and courses, tracking which courses students are enrolled in.

Future Improvements
Implement advanced queries for reporting purposes, such as GPA calculations, course load analysis, and enrollment statistics.

Enhance the schema to include additional features like department management, prerequisites, and course scheduling
