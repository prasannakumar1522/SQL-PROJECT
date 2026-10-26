EVENT TICKET BOOKING SYSTEM – MYSQL PROJECT

 ## Project Overview
The Event Ticket Booking System is a MySQL database project designed to manage users, events, ticket types, and bookings. It stores event details, ticket prices and availability, and booking information.

##Objectives
- Store user and event details.
- Manage ticket types, prices, and available quantities.
- Record bookings and booking status.
- Generate reports using SQL queries.
Technologies Used
- MySQL 8.0
- SQL

##Database Tables
1. users – Stores user and administrator details.
2. events – Stores event information such as title, category, date, time, and location.
3. tickets – Stores ticket types, prices, and available quantities for events.
4. bookings – Stores booking details, quantity, total amount, and booking status.
Table Relationships
- One user can create multiple events.
- One event can have multiple ticket types.
- Users can make bookings for events.
- Each booking is linked to a user, an event, and a ticket type belonging to that event.

##Features
- User and event data management.
- Ticket types, pricing, and availability tracking.
- Booking records with confirmed or cancelled status.
- Queries for upcoming events and category-based searches.
- Booking details using table joins.
- Reports for bookings, revenue, and ticket availability.
- Queries to identify events with no bookings.

##SQL Concepts Used
- CREATE DATABASE and CREATE TABLE
- Primary keys and foreign keys
- AUTO_INCREMENT
- UNIQUE, CHECK, and ENUM constraints
- INSERT and SELECT statements
- WHERE, ORDER BY, and aggregate functions
- INNER JOIN and LEFT JOIN
- GROUP BY and CASE
- COALESCE

##How to Run the Project
1. Open MySQL Workbench or another MySQL 8.0 client.
2. Open the sql_project.txt file.
3. Execute the SQL script.
4. The event_booking_new database and its tables will be created and populated with sample data.
5. Run the included SELECT queries to view the reports.

##Example Reports
- List all users, events, tickets, and bookings.
- Display upcoming events.
- Filter events by category.
- View complete booking details.
- Count bookings for each event.
- Calculate confirmed booking revenue by event.
- Display available ticket types.
- Count bookings by status.
- Find events without bookings.

##Sample Data
The script includes sample records for users, events, ticket types, and bookings to demonstrate the database queries.
Current Limitations
- The sample password values are placeholders, not secure password hashes for production use.
- Ticket availability is stored in the database but is not automatically reduced when a booking is created.
- The project does not currently include views, stored procedures, triggers, or additional explicit indexes.

##Future Improvements
- Add secure user authentication.
- Automatically update ticket availability when bookings are made or cancelled.
- Add views, stored procedures, and triggers.
- Add more validation and reporting features.