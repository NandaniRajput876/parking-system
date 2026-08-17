🚗 Parking Management System
A backend application built using Spring Boot, Spring Data JPA, and MySQL to manage parking-related operations through REST APIs.
The system provides a structured backend for managing parking slots, vehicles, parking entries, and parking records.

📌 Project Overview
The Parking Management System is a Spring Boot REST API application designed to simplify parking management.
The application uses:
Spring Boot for backend development
Spring Web MVC for REST APIs
Spring Data JPA for database operations
Hibernate/JPA for ORM
MySQL for persistent data storage
Maven for dependency management and build
Java 21 as the programming language
The current project configuration is based on Spring Boot 4.1.0, Java 21, Spring Data JPA, Spring Web MVC, and MySQL.

🏗️ Architecture
The application follows a layered Spring Boot architecture: 

               Client
                      |
                      | HTTP Request
                      v
              +----------------+
              |   Controller   |
              +----------------+
                      |
                      v
              +----------------+
              |    Service     |
              +----------------+
                      |
                      v
              +----------------+
              |   Repository   |
              +----------------+
                

Request Flow

               Client
                 ↓
             Controller
                 ↓
              Service
                 ↓
             Repository
                 ↓
           JPA / Hibernate
                 ↓
               MySQL
                 ↓
              Response
                 ↓
               Client

🛠️ Tech Stack
Technology Purpose
Java 21 Programming Language
Spring Boot 4.1.0 Backend Framework
Spring Web MVC REST API Development
Spring Data JPA Database Access
Hibernate ORM
MySQL Database

📂 Project Structure
A recommended structure for the Parking Management System is:

           parking-management-system
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com.example.parkingmanagementsystem
│   │   │       │
│   │   │       ├── controller
│   │   │       │
│   │   │       ├── service
│   │   │       │
│   │   │       ├── repository
│   │   │       │
│   │   │       ├── entity
│   │   │       │
│   │   │       └── ParkingManagementSystemApplication.java
│   │   │
│ │ └ resources


🚘Core Modules
The application can be organized around the following modules.
1. Vehicle Management
Responsible for managing vehicles entering and leaving the parking facility.
Typical operations:

Add Vehicle
Get Vehicle
Update Vehicle
Delete Vehicle

2. Parking Slot Management
Responsible for managing available and occupied parking slots.
Typical operations:

Create Parking Slot
View Parking Slots
Check Slot Availability
Update Slot Status

3. Parking Management
Responsible for maintaining parking records.
A parking record can contain information such as:

Vehicle
Parking Slot
Entry Time
Exit Time
Parking Status

 REST API
The backend exposes REST APIs using Spring Web MVC.
Typical API structure:

POST    /api/vehicles
GET     /api/vehicles
GET     /api/vehicles/{id}
PUT     /api/vehicles/{id}
DELETE  /api/vehicles/{id}

Parking slot APIs:
POST    /api/parking-slots
GET     /api/parking-slots
GET     /api/parking-slots/{id}
PUT     /api/parking-slots/{id}
DELETE  /api/parking-slots/{id}

Parking APIs:
POST    /api/parking
GET     /api/parking
GET     /api/parking/{id}
PUT     /api/parking/{id}
DELETE  /api/parking/{id}

These endpoints are the intended API structure for the README; the uploaded 
files do not currently provide controller implementations to verify exact endpoint 
names.



