# Covid19-Patient-Record-Management-System

## Overview

The Hospital Management System (HMS) is a comprehensive solution designed to manage the various aspects of a hospital's operations. This project aims to streamline the management of patient records, inventory, user roles, and reporting within a hospital setting. The system is built using Java and MySQL, providing a robust and scalable solution for hospital management.

## Features

- **User Management**: Manage different types of users such as doctors, receptionists, and pharmacists.
- **Patient Management**: Record and manage patient details, including personal information and medical history.
- **Inventory Management**: Track and manage hospital inventory, including medical supplies and equipment.
- **Reporting**: Generate various reports for hospital administration and management.
- **Authentication**: Secure login system for different user roles.

## Tech Stack

### Backend
- **Java**: The core programming language used for developing the application.
- **MySQL**: The database management system used to store and manage data.

### Frontend
- **Java Swing**: Used for building the graphical user interface (GUI).

### Build and Deployment
- **Apache Ant**: Used for building and deploying the project.
- **NetBeans**: Integrated Development Environment (IDE) used for development.

## Project Structure

- **src**: Contains the source code for the application.
  - `Main.java`: The main entry point of the application.
  - `Login.form`, `User.form`, `Patient.form`, `Inventory.form`, `Report.form`, `Channel.form`: GUI forms for different modules.
- **nbproject**: Contains NetBeans project files.
  - `project.xml`: Project configuration file.
  - `build-impl.xml`: Generated build script.
  - `project.properties`: Project properties file.
- **.idea**: Contains IntelliJ IDEA project files.
  - `modules.xml`: Module configuration.
  - `vcs.xml`: Version control settings.
  - `misc.xml`: Miscellaneous settings.
  - `Covid19-Patient-Record-Management-System.iml`: Module file.
- **sql**: Contains SQL dump files for database setup.
  - `loyalhospital_user.sql`: SQL script for the `user` table.
  - `loyalhospital_patient.sql`: SQL script for the `patient` table.
  - `loyalhospital_item.sql`: SQL script for the `item` table.

## Prerequisites

- Java Development Kit (JDK) 19
- MySQL Server
- Apache Ant
- NetBeans IDE (optional but recommended)

## Installing Dependencies

### Java Development Kit (JDK)

1. **Download JDK 19**: Download the JDK from the [official Oracle website](https://www.oracle.com/java/technologies/javase-jdk19-downloads.html).
2. **Install JDK**: Follow the installation instructions for your operating system.

### MySQL Server

1. **Download MySQL Server**: Download MySQL Server from the [official MySQL website](https://dev.mysql.com/downloads/mysql/).
2. **Install MySQL Server**: Follow the installation instructions for your operating system.

### Apache Ant

1. **Download Apache Ant**: Download Apache Ant from the [official Apache Ant website](https://ant.apache.org/bindownload.cgi).
2. **Install Apache Ant**: Follow the installation instructions for your operating system.
3. **Set Environment Variables**:
   - Add `ANT_HOME` to your system environment variables, pointing to the Ant installation directory.
   - Add `ANT_HOME/bin` to your system `PATH`.

### MySQL Connector/J

1. **Download MySQL Connector/J**: Download the MySQL Connector/J JAR file from the [official MySQL website](https://dev.mysql.com/downloads/connector/j/).
2. **Add to Project**:
   - In NetBeans, right-click on the project and select `Properties`.
   - Go to `Libraries` and click `Add JAR/Folder`.
   - Select the downloaded MySQL Connector/J JAR file and add it to the project.

## Setup Database

1. **Start MySQL Server**: Ensure that your MySQL server is running.
2. **Create Database**: Create a new database named `loyalhospital`.
3. **Import SQL Scripts**:
   - Open MySQL command line or a MySQL client (e.g., MySQL Workbench).
   - Run the following commands to import the SQL scripts:
     ```sql
     SOURCE path/to/loyalhospital_user.sql;
     SOURCE path/to/loyalhospital_patient.sql;
     SOURCE path/to/loyalhospital_item.sql;
     ```

## Build and Run the Project

1. **Clone the Repository**: Clone the project repository to your local machine.
2. **Open in NetBeans**: Open the project in NetBeans IDE.
3. **Build the Project**: Use NetBeans to build the project or run the following command in the project directory:
   ```sh
   ant clean build
   ```
4. **Run the Project**: Use NetBeans to run the project or run the following command:
   ```sh
   ant run
   ```

### Configuration

- **Database Configuration**: Ensure that the MySQL connector JAR is correctly referenced in the project properties file.
  ```LoyalHospital/nbproject/project.properties
  startLine: 38
  endLine: 43
  ```

- **Main Class**: The main class for the application is specified in the project properties.
  ```LoyalHospital/nbproject/project.properties
  startLine: 79
  endLine: 79
  ```

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact

For any questions or support, please contact Onkar at andurkaronkar@gmail.com
