# User Management Interface
<ol>
<li>Introduction
  <ol>
    <li>Purpose</li>
    <li>Indented Audience</li>
    <li>Indented Use</li>
    <li>Scope</li>
    <li>Definitions and Acronyms</li>
  </ol>
</li>
<li>System Features and Requirements
  <ol>
    <li>Functional Requirements</li>
    <li>Nonfunctional Requirements</li>
  </ol>
</li>
<li>UI Components
  <ol>
    <li>Left Side</li>
    <li>Right Side</li>
  </ol>
</li>
<li>Initial State
</li>
</ol>

## Introduction
User Creation Tool. A web portal allowing admins to view existing users and create new ones.
### Purpose
The purpose of this software to easily create new users and save them to a database.
### Intended Audience
The main users of this software are IT personnels.
### Intended Use
The main use of this software is to create and save new users with different roles.
### Scope
This software makes it easy to create new users: instead of writing an SQL query every time for each new user, you can fill the text boxes and click a button to create a new user. This can save lots of time if there are many users to crate.
### Risks
The users of this software must be really careful when creating new users. If they give admin roles to standard guest users, there may be huge security issues.

## System Features and Requirements
### Functional Requirements
- Software sends and retrieves information from a database. The software must be connected to a server via the database so user list always keep updated for everyone in the company.  
- The table retrieves the users table from the database.  
- New user button enables the text boxes to be filled.  
- Save user button generates a SQL query that inserts a new row to users table based on the information written in the text boxes. After saving, text boxes will be greyed out.  
- Hide disabled users checkbox hides the users from the table with the Enabled value as false.  
- Table can be sorted via clicking the column names.  
### Nonfunctional Requirements
- The user creation must be reliable and show that user successfully created.  
- The software must be easy to maintain and use.

## UI Components
### Left Side
#### Buttons
***New User:*** Makes the greyed out textboxes in the right to be writable.
#### Checkboxes
***Hide Disabled User:*** Hides the users from the Users Table with the Enabled value as false when checked.
#### Tables
***Users Table:*** Shows information about Users table from the database.
### Right Side
#### Buttons
***Save User:*** Inserts the user to the database with the information written in the textboxes. After saving, it makes text boxes greyed out again.
#### Textboxes
***Username, Display Name, Phone, Email:*** User information to be filled by the software user.
#### Checkboxes
***Enabled:*** When checked, it saves the user with the Enabled value as true.

## Inital State
The user of the software will encounter a window with the Users table on the left that lists all users and grayed-out text boxes on the right. The text boxes will be available once the New User button is clicked.
