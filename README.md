# Hotel Management System (Java + MySQL)

A **console-based Hotel Management System** built using **Java** and **MySQL**.  
This project allows hotel staff to manage reservations with CRUD operations via a simple text-based menu.

---

## Features
- Reserve a Room (Insert new reservation)  
- View Reservations (Display all reservations in tabular format)  
- Get Room Number (Fetch room number using Reservation ID and Guest Name)  
- Update Reservation (Modify guest name, room number, or contact)  
- Delete Reservation (Remove a reservation by ID)  
- Exit with countdown animation  

---

## Requirements
- Java JDK 8+  
- MySQL Database  
- MySQL Connector/J (JDBC Driver)  

---

## Setup
1. Create a MySQL database:
   ```sql
   CREATE DATABASE hotel_db;
   USE hotel_db;

   CREATE TABLE res (
       res_id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       room_no INT NOT NULL,
       contact_no VARCHAR(15) NOT NULL,
       res_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );

