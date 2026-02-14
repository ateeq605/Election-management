# Web-Based Election Systems

**Web-Based Voting Management System**

## Project Overview

The **Web-Based Election Systems** is a web-based application developed using PHP and MySQL to manage election processes digitally. The system allows administrators to manage candidates, voters, positions, and election results through a centralized dashboard.

This project demonstrates the design, development, and testing of a working artefact for the MSc Computer Science project submission.

## Problem Statement

Manual election result management systems are time-consuming, error-prone, and inefficient. Institutions require a digital system that can securely manage voting data, candidates, and results while providing accurate vote counting. This project addresses these challenges by providing an automated election result management system.

## Project Objectives

- Develop a functional election management system.
    
- Implement admin authentication.
    
- Manage candidates, voters, and positions.
    
- Allow ballot submission.
    
- Store votes securely in a database.
    
- Generate election results.
    
- Provide a user-friendly interface.
    

* * *

## System Features

### Admin Features

- Admin login/logout & Dashboard overview
    
- **Candidate Management:** Add, Edit, and Delete candidates
    
- **Voter Management:** Add, Edit, and Delete voters
    
- **Position Management:** Define election roles
    
- **Monitoring:** Real-time vote monitoring and result preview
    
- **Maintenance:** Reset votes and Print results (PDF)
    

### User Features

- Ballot preview
    
- Secure vote submission
    
- Result viewing
    

* * *

## System Architecture

Plaintext

```
Browser (Client Interface) 
      ↓ 
Apache Server (XAMPP) 
      ↓ 
PHP Application Logic 
      ↓ 
MySQL Database
```

## Technologies Used

- **Frontend:** HTML, CSS, Bootstrap, JavaScript
    
- **Backend:** PHP
    
- **Database:** MySQL
    
- **Libraries:** TCPDF (PDF generation)
    
- **Environment:** XAMPP, VS Code, Git & GitHub
    

* * *

## Project Folder Structure

Plaintext

```
ElectionResults_system/
│
├── admin/          # Admin panel files
├── database/       # SQL dump files
├── db/             # Database connection logic
├── includes/       # Reusable components (header/footer)
├── images/         # Static assets
├── plugins/        # Third-party plugins
├── dist/           # Compiled CSS/JS
├── tcpdf/          # PDF Generation library
├── index.php       # Voter Login/Landing
├── login.php       # Authentication logic
├── submit_ballot.php
└── home.php        # Voter Dashboard
```

* * *

## Installation Guide

### Step 1: Install XAMPP

Install XAMPP and start the **Apache** and **MySQL** services.

### Step 2: Copy Project

Copy the project folder into your htdocs directory:

`C:\xampp\htdocs\`

### Step 3: Import Database

1.  Open [http://localhost/phpmyadmin](https://www.google.com/search?q=http://localhost/phpmyadmin)
    
2.  Create a new database named: `votesystem`
    
3.  Import the SQL file located at: `database/votesystem.sql`
    

### Step 4: Run the Application

- **User Interface:** [http://localhost/ElectionResults_system](https://www.google.com/search?q=http://localhost/ElectionResults_system)
    
- **Admin Panel:** [http://localhost/ElectionResults_system/admin](https://www.google.com/search?q=http://localhost/ElectionResults_system/admin)
    

**Default Admin Login:**

> **Username:** sadam
> 
> **Password:** password

* * *

## Testing Strategy

Testing was performed on all core modules to ensure the integrity of the voting process.

| **Test Case** | **Expected Result** | **Outcome** |
| --- | --- | --- |
| Admin Login | Dashboard loads successfully | **Pass** |
| Add Candidate | Candidate saved to database | **Pass** |
| Submit Ballot | Vote stored and linked to voter | **Pass** |
| View Results | Correct totals displayed dynamically | **Pass** |

* * *

## Limitations & Future Improvements

### Limitations

- No email authentication for voters.
    
- Plain text/simple password storage (no high-level encryption).
    
- Localhost deployment only.
    
- No multi-admin support.
    

### Future Improvements

- Implementation of password encryption.
    
- Cloud deployment and mobile responsive UI.
    
- Real-time results dashboard and API integration.
    
- Role-based access control.
    

* * *

## GitHub Repository

[GitHub Link](https://github.com/ateeq605/ElectionResult-system)

## Author

**Ateeq ur Rehman**

## License

This project is developed for academic purposes.
