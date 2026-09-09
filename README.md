Task Management · Hail Region Municipality

A classic, data-focused task management portal designed to coordinate departmental work for the Hail Region Municipality.

The interface is built with HTML, CSS, and Vanilla JavaScript, while PHP powers the backend with a MySQL database. The project is fully compatible with MAMP on macOS.

⸻

Key Features

* Secure Authentication
    Role-based authentication for Presidents, Managers, and Employees.
* Dashboard
    A concise overview of key metrics, upcoming deadlines, and reminder history presented in a classic two-column layout.
* Task Management
    Dedicated task creation workspace with a streamlined task roster, inline status updates, and reminder triggers.
* Calendar
    Monthly calendar view for visualising departmental deadlines with colour-coded priorities and quick monthly statistics.
* Department Directory
    Centralised directory containing department information, optional contact details, and workload summaries for the fourteen provided departments.
* Reminder Management
    Dedicated reminder hub for creating follow-up notices and reviewing reminder history.

⸻

Requirements

Before running the project, make sure you have:

* PHP 8.0 or newer
* MySQL
* Apache or another compatible web server
* MAMP on macOS

⸻

Getting Started with MAMP

1. Copy the Project

Place the project inside your MAMP web directory:

/Applications/MAMP/htdocs

2. Open phpMyAdmin

Open:

http://localhost/phpMyAdmin

3. Import the Database

Import the database schema located at:

database/schema.sql

The schema creates the required tables and seeds:

* Departments
* Tasks
* Calendar events
* Notifications
* Three demo user accounts

4. Configure the Database

Open:

db.php

Update the connection values if your MySQL credentials differ.

The default MAMP credentials are:

Username: root
Password: root
Database: task_manager

5. Start the Application

Start the Apache and MySQL servers through MAMP.

Then open:

http://localhost/tatarwar/login.php

If you used a different project folder name, replace tatarwar with your folder name.

6. Sign In

You can sign in using one of the seeded accounts or create a new account through the registration page.

Demo Accounts

Role	Email	Password
President	president@hailtasks.test	president123
Manager	manager@hailtasks.test	manager123
Employee	employee@hailtasks.test	employee123

⸻

Database Structure

users

Authentication table containing user roles, hashed passwords, and audit timestamps.

departments

Stores department names and optional email contact information.

tasks

Tracks task details, responsible departments, priorities, statuses, and due dates.

notifications

Stores reminder messages associated with tasks.

calendar_events

Stores calendar items used to populate the monthly schedule view.

⸻
## Project Structure

```text
├── assets
│   ├── css
│   │   └── style.css
│   └── js
│       └── app.js
├── database
│   └── schema.sql
├── includes
│   ├── footer.php
│   ├── functions.php
│   └── header.php
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

## Classic Design Accents

### Gradient Shell
A linear gradient background combined with frosted surfaces creates a timeless control-room aesthetic.

### Summary Cards & Tables
Reusable cards and elevated tables keep metrics, statuses, and priorities easy to scan.

### Dedicated Flows
Separate screens for reminders and task creation provide straightforward navigation while keeping the interface organised.
⸻

Classic Design Accents

Gradient Shell

A linear gradient background combined with frosted surfaces creates a timeless control-room aesthetic.

Summary Cards & Tables

Reusable cards and elevated tables keep metrics, statuses, and priorities easy to scan.

Dedicated Hubs

Separate screens for reminders and task creation provide straightforward navigation while keeping the interface organised.

Responsive Layout

The layout adapts gracefully to smaller screens while preserving the primary navigation and key performance indicators.

⸻

Customisation Tips

Styling

Adjust typography, spacing, and colour palettes inside:

assets/css/style.css

to match your preferred branding.

Reminder Integrations

Extend:

send_reminder.php

to support external notification services such as:

* Email
* SMS
* Chat integrations

Additional Metadata

Add new fields to the forms in:

task_create.php
departments.php

and update:

database/schema.sql

accordingly.
