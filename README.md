📌 Project Description

This project is a Windows Forms desktop application developed to manage films, genres, and directors along with their relationships.
The application follows N-Tier Architecture principles and communicates with a SQL Server database using Entity Framework Core.

The system allows users to perform:

Add, delete, update, and search films

Add, delete, update, and search genres

Add, delete, update, and search directors

📌 Technologies Used

C# Programming Language

.NET Platform

Windows Forms

Entity Framework Core

Microsoft SQL Server

SQL Server Management Studio

N-Tier Architecture

Generic Repository Pattern

Service (Business Logic) Layer

📌 Project Architecture
📌 Models (Entities) Layer

This layer contains the entity classes that represent database tables.

Film

Genre (Tur)

Director (Yonetmen)

It only defines data structures and does not include business logic.

📌 DAL – Data Access Layer

Responsible for direct communication with the database.

DbContext configuration

Entity Framework Core operations

Generic Repository implementation

All CRUD operations are handled in this layer.

📌 BLL – Business Logic Layer

This layer contains the application’s business rules.

FilmService

TurService

YonetmenService

It acts as a bridge between the UI and the data access layer.

📌 PL – Presentation Layer

This layer represents the user interface of the application.

Windows Forms UI

Handles user interactions

Displays data using DataGridView and ComboBox controls

📌 Database Relationships

One Genre can have multiple Films (1-N)

One Director can have multiple Films (1-N)

Each Film is associated with one Genre and one Director

📌 Key Features

Clean and maintainable layered architecture

Reduced code duplication using Generic Repository pattern

ORM-based database operations with Entity Framework Core

Safe delete and update operations using ID-based validation

Relationship checks before delete operations

📌 Setup Instructions

Clone or download the repository

Create the database using SQL Server

Update the connection string according to your environment

Run the project using Visual Studio
