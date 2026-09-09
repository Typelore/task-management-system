Task Management System · Hail Region Municipality

A full-stack task management system designed to help departments organise, track, and manage their day-to-day work.

The system provides role-based access, task management, deadline tracking, calendar scheduling, department management, and reminders through a centralised web application.

⸻

Overview

The Task Management System was developed for the Hail Region Municipality to provide a structured way of managing departmental tasks and monitoring their progress.

The application is built around three user roles — President, Manager, and Employee — with role-based access to the system’s features.

The project combines a PHP backend with a MySQL database and a responsive frontend built using HTML, CSS, and Vanilla JavaScript.

⸻

Features

🔐 Role-Based Authentication

* Secure user authentication
* Three user roles: President, Manager, and Employee
* Role-based access to system functionality
* Password hashing and user management

📊 Dashboard

* Overview of task statistics
* Upcoming deadlines
* Task status summaries
* Recent reminder activity

📋 Task Management

* Create and manage tasks
* Assign tasks to departments
* Set priorities and due dates
* Track task status
* Trigger reminders for upcoming deadlines

📅 Calendar

* Monthly calendar view
* Visual deadline tracking
* Priority indicators
* Monthly task and event statistics

🏢 Department Directory

* Centralised department information
* Contact details
* Department workload summaries
* Support for the fourteen provided departments

🔔 Reminder Management

* Create task reminders
* Manage follow-up notifications
* Review reminder history
* Connect reminders to specific tasks

⸻

Tech Stack

Technology	Purpose
HTML	Application structure
CSS	Styling and responsive interface
JavaScript	Client-side interactions
PHP	Backend logic and server-side functionality
MySQL	Database management
MAMP	Local development environment

⸻

##Application Structure
```text
task-management/
│
├── assets/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── app.js
│
├── database/
│   └── schema.sql
│
├── includes/
│   ├── footer.php
│   ├── functions.php
│   └── header.php
│
├── calendar.php
├── db.php
├── departments.php
├── index.php
├── login.php
├── logout.php
├── reminders.php
├── register.php
├── send_reminder.php
├── task_create.php
├── tasks.php
└── README.md
```
The project follows a modular structure, separating frontend assets, database files, reusable PHP components, and application pages.

⸻

Database

The application uses MySQL to manage users, departments, tasks, notifications, and calendar events.

Main Tables

* users — authentication, roles, and account information
* departments — department information and contact details
* tasks — task details, priorities, statuses, and deadlines
* notifications — task-related reminders
* calendar_events — scheduled events and calendar data

⸻

Getting Started

Requirements

Before running the project, make sure you have:

* PHP 8.0+
* MySQL
* Apache
* MAMP on macOS

1. Setup the Project

Place the project inside the MAMP web directory:

/Applications/MAMP/htdocs

2. Start MAMP

Start both Apache and MySQL from MAMP.

3. Import the Database

Open phpMyAdmin:

http://localhost/phpMyAdmin

Import:

database/schema.sql

The schema includes the required tables and demo data.

4. Configure the Database

Open:

db.php

The default MAMP configuration is:

Username: root
Password: root
Database: task_manager

Update these values if your local configuration is different.

5. Launch the Application

Open:

http://localhost/<project-folder>/login.php

Replace <project-folder> with the project folder name.

⸻

Demo Accounts

Role	Email	Password
President	president@hailtasks.test	president123
Manager	manager@hailtasks.test	manager123
Employee	employee@hailtasks.test	employee123

⸻

Design

The interface uses a clean administrative dashboard layout focused on readability and efficient navigation.

The application includes:

* Responsive layouts
* Dashboard summary cards
* Structured data tables
* Dedicated task and reminder pages
* Monthly calendar interface
* Consistent navigation across the application

⸻

Future Improvements

Potential extensions for the system include:

* Email and SMS notification integrations
* Advanced task filtering and search
* Detailed reporting and analytics
* File attachments for tasks
* Expanded permission management
* Activity and audit logs

⸻

Project Purpose

This project demonstrates the development of a full-stack web application using PHP and MySQL, with practical implementation of authentication, role-based access, database relationships, CRUD operations, task management, and responsive interface design.
