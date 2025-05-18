<h1 align="center">FormaNT RENTAL CARS</h1>
FormaNT - Rental Cars is a Java-based web application that allows a user to register and rent a car. The user can choose the car they want to rent, the start and end date of the rental.

<hr/>

# 🚗 Application

- Search page: users can search for cars by filtering through various parameters;
- Check reservations: users can verify the reservations made by each user;
- Login System: users can register and log in to the application;
- Edit/Update System: cars can be added, edited, and removed, and users can be added, edited, and removed.

<hr/>

# 🚗 Technology

FormaNT - Rental Cars is built using the following technologies:

BACKEND:
- Java: version 17;
- PostgreSQL: version 7.2;
- Spring Boot: version 3.1.2;

<hr/>

# 🚗 How to run the project

## Step 1: Download and extract the code

First, download the website code and extract the ZIP file to a folder on your local system.

## Step 2: Make the necessary configurations

### 🐘 Configure the database
This application uses PostgreSQL as its DB. You will need to install the system and create a database for the application.

🚨 NOTE: The database is configured in the project to run on port 5432. If you are using a different port, change the "application.properties" file to the port you are using.

- PORT: 5432
- USER: postgres
- PASSWORD: password

## Step 3: Run your project

Open your code editor (such as IntelliJ), navigate to the project directory, and run the application.

<hr/>

### ✨ Code indentation

When you perform a commit in Git, the code is automatically formatted to follow an indentation standard.

🚨 NOTE: However, for the formatting to be applied, Git automatically executes the command "git add .", even if you have modified only one file using "git add 'filename'", Git will actually perform a "git add ." to include all pending changes in the commit, including the formatting changes. Therefore, it is important to make sure that you have made only the necessary changes before performing the commit, as all changes, including formatting, will be included.

For automatic indentation to work, it is necessary to modify the pre-commit.sample file in the FormaNT/.git/hooks directory.

- Open the pre-commit.sample file in a text editor.
- Delete everything in this file and paste the following code:
```
#!/bin/bash
./pre-commit.sh
```
- Rename the file by removing ".sample" and leaving only "pre-commit".
- Now, after "git commit", the "pre-commit.sh" file in the project root will be executed.

<hr/>

# 🚨 Important Warnings

- 🚨 Tomcat is configured to run on port 8080, so in addition to PostgreSQL on port 5432, make sure you don't have any other application running on this port (8080). If there is, make the necessary changes (application.properties).
- 🚨 The project already comes with some dependencies pre-installed. If it is necessary to make changes, remember that it was developed following the configurations above.
