# Orphanage Management System 

## Description
The Orphanage Management System is a web-based platform designed to manage orphan registrations, donations, and secure data transactions efficiently. Built using PHP with Object-Oriented Programming (OOP) and design patterns, this system ensures scalability, maintainability, and security.

## Features
**User Authentication & Security:** Secure login system for admins and donors.

**Orphan Management:** CRUD operations for registering, updating, and deleting orphan records.

**Donation Tracking:** Tracks and manages donations made by sponsors.

**Secure Transactions:** Utilizes hashing and encryption for secure data storage.

**Role-Based Access Control (RBAC):** Ensures different permissions for admins, staff, and donors.

**Efficient Database Handling:** Uses MySQL for structured data management.

**Modular Design:** Implements functions.php and OOP classes for reusable code.

## Design Patterns Used
This project follows key software design patterns to enhance scalability and maintainability:

**Singleton Pattern**

-Ensures a single database connection instance throughout the application.

-Implemented in link.php for managing MySQL connections.

**Factory Pattern**

-Used for creating different user roles (Admin, Donor, Orphan) dynamically.

-Centralized object creation reduces redundancy and improves maintainability.

**Facade Pattern**

-Provides a simplified interface to complex operations like donation processing, authentication, and orphan record management.

-Helps in hiding complexities and improving code readability.

**Single Usage Pattern**

-Used to restrict multiple instances of certain objects in the system, ensuring unique operations.

-Prevents redundancy in user session management, database transactions, and orphan record validation.

**MVC (Model-View-Controller) Structure**

-Models handle database interactions.

-Views manage UI rendering (HTML, CSS).

-Controllers process user requests and coordinate between models and views.

**Strategy Pattern**

-Implements different hashing techniques for securing passwords and sensitive data.

-Allows easy switching between bcrypt, SHA-256, or Argon2.

**Observer Pattern**

-Used for notifications when a new orphan record is created or a donation is made.

-Keeps the system loosely coupled for future enhancements.

**Decorator Pattern**

-Enhances user roles with additional permissions dynamically.

-Applied in the RBAC (Role-Based Access Control) system.

## Technology Stack
**Backend:** PHP (OOP + Design Patterns)

**Database:** MySQL

**Frontend:** HTML, CSS, JavaScript

**Security:** Hashing, Data Encryption
## Project Structure
```bash
/orphanage-system/
│-- index.php              # Homepage
│-- checkid.php            # ID verification script
│-- checksecid.php         # Secure ID checker
│-- createdondet.php       # Donation processing
│-- functions.php          # Core functions (OOP utilities)
│-- link.php               # Database connection
│-- page.php               # Pagination & UI rendering
│-- testhashing.php        # Hashing & encryption test
│-- assets/                # CSS, JS, Images
│-- database/              # SQL schema & backups
│-- classes/               # PHP OOP classes
```
