🚗 Parking Management System:


A backend application built using Spring Boot, Spring Data JPA, and MySQL to manage parking-related operations through REST APIs.


The system provides a structured backend for managing parking slots, vehicles, parking entries, and parking records.

📌 Project Overview:


The Parking Management System is a Spring Boot REST API application designed to simplify parking management.
The application uses:


- Spring Boot for backend development


- Spring Web MVC for REST APIs


- Spring Data JPA for database operations


- Hibernate/JPA for ORM


- MySQL for persistent data storage


- Maven for dependency management and build


- Java 21 as the programming language

🏗️ Architecture:


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

🛠️ Tech Stack:

![image alt](https://github.com/NandaniRajput876/parking-system/blob/54852cc07b45a348a9f74483ef823d0c484b2eda/WhatsApp%20Image%202026-08-18%20at%2002.29.46.jpeg)

📂 Project Structure:

A recommended structure for the Parking Management System is:

![image alt](https://github.com/NandaniRajput876/parking-system/blob/5ce0248e68bae3b6feffaf02933ffec50ff591e6/project_structure.jpeg)
 
🚘 Core Modules:

The application can be organized around the following modules.

Vehicle Management:
Responsible for managing vehicles entering and leaving the parking facility.

→ Typical operations:

a) Add Vehicle

b) Get Vehicle

c) Update Vehicle

d) Delete Vehicle

Parking Slot Management:
Responsible for managing available and occupied parking slots.

→ Typical operations:

a) Create Parking Slot

b) View Parking Slots

c) Check Slot Availability

d) Update Slot Status

→ Example slot states:

a) AVAILABLE

b) OCCUPIED

Parking Management:
Responsible for maintaining parking records.

A parking record can contain information such as:

a) Vehicle

b) Parking Slot

c) Entry Time

d) Exit Time

e) Parking Status

🌐 REST API:

The backend exposes REST APIs using Spring Web MVC.

Typical API structure:

Parking slot APIs:

Parking APIs:

🗄 Database:

The application uses MySQL as its database. 

Spring Data JPA is used to communicate with the database.

The project includes the MySQL Connector/J runtime dependency in pom.xml.



