 # Task 1:  Flask Application
This is a Flask web application that demonstrates basic CRUD operations with a MySQL database. It includes functionalities to list users, add new users, and view user details.
## Features
 - View a list of users
 - Add new users
 - View details of a specific user
 - Simple user interface using HTML templates

## Setup Instructions
- Prerequisites
- Python 3.x installed on your machine
- Flask installed (`pip install flask`)
- MySQL installed and running
 
### Installation
1. Clone the repository:
   - git clone https://github.com/VirendraMekhle/flask_app.git
   
2. Navigate to the project directory:
   - cd flask_app
   
3. Create and activate a virtual environment (optional but recommended):
    - python -m venv venv 
    - venv\Scripts\activate

4. Install dependencies:
   - pip install -r requirements.txt

5.Set up the database:
   # Database configuration
    db_config = {
    'user': 'database_username', for mine  [username: root & password: admin]
    'password': 'yourpassword',
    'host': 'localhost',
    'database': 'users'
  }
 
6. Run the application:
  - flask run
  
7. Access the application:
   - http://127.0.0.1:5000/hello
   - http://127.0.0.1:5000/users 
   - http://127.0.0.1:5000/new_user
   - http://127.0.0.1:5000/users/1

# Task 2:  DataBase Scheme
   1.     CREATE DATABASE users;
          USE users;

   2.     CREATE TABLE users (
          id INT AUTO_INCREMENT PRIMARY KEY,
          name VARCHAR(255),
          email VARCHAR(255),
          role VARCHAR(255));
          
   3.     INSERT INTO users (NAME, email, ROLE) VALUES
           ('Virendra Kumar', 'vmekhle@gmail.com', 'Admin'),
           ('Gagan Sahu', 'gsahu@gmail.com', 'User'),
           ('Mohit Sahu', 'mohitsahu@gmail.com', 'Manager');
         
          Retrieve all users from the "users" table: 
           - Select * From users;
        
          Retrieve a specific user by their ID: 
           - Select name , email , role  OR [Select *]
             from users
             where id = 1;

 # Task 3:  Git WorkFlow
        1. Clone the repository
           - git clone https://github.com/VirendraMekhle/flask_app.git
        2.Create a new branch:
            - git checkout -b branch_name
        3.Make changes and commit
            - git add .
            - git commit -m "Describe your changes"
        4.Push changes to the remote repository:
            - git push origin branch_name
        5.Create a Pull Request on GitHub:
           Go to the "Pull requests" tab on GitHub.
           Click "New pull request" and select your branch to merge into the main branch.
           Follow the instructions to create and review the pull request.
        
 ## Dependencies
        - Flask
        - MySQL Connector
        - Python packages listed in requirements.txt

  ## Troubleshooting
        - MySQL server is running and accessible.
        - Verify the database connection settings in the Flask app.

  
