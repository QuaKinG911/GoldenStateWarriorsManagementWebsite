# Golden State Warriors Management System

A web-based management system designed for the Golden State Warriors NBA team to track team and player statistics, schedules, and performance data.

## Features

- **Player Management**: Add, update, and delete player profiles, including key details like player statistics, personal information, and performance history.
- **Game Schedule Tracking**: Manage the team's upcoming games, including dates, times, opponents, and results.
- **Team Performance Overview**: Generate reports on team performance, including win/loss records and player statistics.
- **Database Integration**: MySQL database to store and manage team and player data.
- **User Authentication**: Secure login system for admins and authorized personnel to manage team data.
- **Responsive Interface**: User-friendly interface designed using HTML, CSS, and JavaScript to ensure smooth navigation on various devices.

## Technologies Used

- **Backend:** JSP (JavaServer Pages)
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Authentication:** Simple user authentication with roles for admins

## Installation

### Prerequisites
Ensure you have the following installed:
- Java 8 or higher
- Apache Tomcat server
- MySQL

### Steps

1. **Download the project**:  
   Download the project ZIP file from the GitHub repository:  
   - [GoldenStateWarriorsManagementWebsite](https://github.com/QuaKinG911/GoldenStateWarriorsManagementWebsite)

2. **Unzip the file**:  
   After downloading the `.rar` file, unzip it. You will find the following contents:
   - The project code
   - The MySQL database (`Dump20240620.sql`)
   - A full report

3. **Set up MySQL Database**:  
   - Create a database in MySQL and import the provided database file (`Dump20240620.sql`).
   
     ```sql
     CREATE DATABASE gsw_management;
     USE gsw_management;
     SOURCE path/to/Dump20240620.sql;
     ```

4. **Configure Database Connection**:  
   Edit the `database-config.properties` file in the extracted project folder to match your MySQL credentials (username, password, database name).

5. **Deploy the Project to Apache Tomcat**:  
   - Copy the extracted project folder into the `webapps` directory of your Tomcat server.
   - Start the Tomcat server by running the following command:

     ```bash
     ./startup.sh   # For Linux/macOS
     startup.bat    # For Windows
     ```

6. **Access the Application**:  
   Open your browser and go to:

   ```
   http://localhost:8080/GoldenStateWarriorsManagementWebsite
   ```

## Usage

- **Admin Login**: Use the admin credentials provided in the `credentials.txt` file to access the management interface.
- **Player and Game Management**: After logging in, navigate to the "Player Management" and "Game Schedule" tabs to add, edit, or delete records.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push the branch (`git push origin feature-name`).
5. Open a Pull Request.

