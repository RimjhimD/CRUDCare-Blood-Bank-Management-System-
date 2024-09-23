# CRUDCare - Blood Bank Management System

## Project Overview

CRUDCare is a web-based Blood Bank Management System designed to streamline and optimize the operations of a blood bank. It facilitates easy management of donor information, blood donations, blood inventory, and blood requests from hospitals. Additionally, it provides functionalities for lab technicians to manage blood tests, and hospital representatives to request blood for patients. Admins oversee the users and manage the operations of the blood bank system.

Developed with PHP, SQL, HTML, CSS, and Bootstrap, CRUDCare enhances the efficiency of blood bank operations by automating key tasks and ensuring seamless interaction between the blood bank and hospital representatives.

## Features

CRUDCare includes the following core features:

### 1. Admin Dashboard
- Manage users (donors, recipients, lab technicians, hospital representatives).
- Oversee blood donations and requests.
- Configure system settings.
- Sidebar navigation with collapsible menu for ease of use.

### 2. Donor Dashboard
- Register and update personal information.
- Schedule and view blood donation history.

### 3. Recipient Dashboard
- Request blood from available inventory.
- View request status and history.

### 4. Lab Technician Dashboard
- Test and update the status of blood donations.
- View and manage blood test results.

### 5. Inventory Manager Dashboard
- Manage blood inventory (add, update, and remove blood units).
- Monitor blood stock levels and expiry dates.

### 6. Hospital Representative Dashboard
- Make blood requests on behalf of patients.
- View status and fulfillment of blood requests.

## Technology Stack

- **Frontend**: HTML, CSS, Bootstrap
- **Backend**: PHP
- **Database**: MySQL
- **Version Control**: Git
- **Local Development**: XAMPP

## Installation and Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/crudcare-blood-bank-management.git
    ```

2. **Set up XAMPP**:
    - Install XAMPP (if not already installed).
    - Start **Apache** and **MySQL** from the XAMPP control panel.

3. **Create the database**:
    - Open `phpMyAdmin` at `http://localhost/phpmyadmin`.
    - Create a new database, for example: `crudcare_db`.
    - Import the provided SQL file located in `database/crudcare_db.sql` to set up the necessary tables.

4. **Configure the database connection**:
    - Open the project folder.
    - Go to `config/db_config.php` and set your database connection details:
        ```php
        $db_host = 'localhost';
        $db_user = 'root';
        $db_password = '';  // Set your password if any
        $db_name = 'crudcare_db'; // The name of your database
        ```

5. **Access the system**:
    - Start your local server by placing the project folder in `htdocs` (XAMPP).
    - Access the system in your browser at `http://localhost/crudcare-blood-bank`.

6. **Login credentials**:
    - Admin and other user roles should be created through the system.
    - Default login credentials for admin:
      - Username: `admin`
      - Password: `admin`

## System Architecture

CRUDCare is structured into different modules, each with its own functionality:

- **Admin Module**: Manages users (donors, recipients, lab technicians, hospital representatives).
- **Donor Module**: Handles donor registration, scheduling donations, and viewing donation history.
- **Recipient Module**: Allows recipients to request blood and view request history.
- **Inventory Module**: Managed by the inventory manager to keep track of blood stock.
- **Lab Technician Module**: Manages blood testing and updates test results for donations.
- **Hospital Representative Module**: Allows hospital representatives to place and track blood requests.

## Database Schema

CRUDCare uses the following key database tables:

- `users`: Stores data for all system users (admins, donors, recipients, hospital representatives, lab technicians, etc.).
- `donations`: Manages records of blood donations made by donors.
- `blood_units`: Tracks available blood in inventory.
- `blood_requests`: Handles blood requests made by hospital representatives.
- `blood_test_results`: Stores results of blood tests conducted by lab technicians.
- `locations`: Holds information about the locations where blood is stored or where donations can be made.
- `lab_technician_info`: Stores information about lab technicians who handle blood testing.
- `inventory`: Manages the inventory of blood units.
- `hospital_representative_info`: Contains information about hospital representatives who request blood.

## Authors

This project was developed by:

- **(@MohammadSakib)
- **(@Sharif1023)
- **(@Shadman02)
- **(@NishadulIslam)
- **(@RimjhimDey)

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit and push your changes (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
