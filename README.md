# Basketball Website

A modern, interactive basketball-themed website designed for players and enthusiasts to explore tournaments, improve their skills, and stay connected.

## Features

### Frontend
- **Homepage:**
  - Eye-catching animations and a basketball-themed layout.
  - Inspirational quotes to motivate users.
  - Search functionality for quick access.
- **Navigation:**
  - Accessible menu options for:
    - Home
    - Tournaments
    - Gallery
    - Login
    - Contact Us
- **Styling:**
  - Fully responsive design.
  - Background image with a basketball aesthetic.
  - Font styles from Google Fonts for a professional look.
- **Animations:**
  - Slide-in animations for engaging user experience.

### Backend
- **Database Integration:**
  - MySQL database to store user information securely.
  - Example database table: `users` with fields `id`, `username`, `password`, `email`, and `created_at`.
- **User Management:**
  - Add, retrieve, update, and delete user information using Java-based APIs.
  - Password handling (note: implement password hashing for production).

## Requirements

### Frontend
- A modern browser supporting HTML5, CSS3, and JavaScript.

### Backend
- Java Development Kit (JDK 8 or later).
- MySQL server.
- JDBC driver.

## Setup

### Frontend
1. Place the HTML, CSS, and JavaScript files in your web server's root directory.
2. Ensure all paths to assets (e.g., images, fonts) are correct.

### Backend
1. Set up the MySQL database:
   ```sql
   CREATE DATABASE user_database;
   USE user_database;
   CREATE TABLE users (
       id INT AUTO_INCREMENT PRIMARY KEY,
       username VARCHAR(50) NOT NULL,
       password VARCHAR(255) NOT NULL,
       email VARCHAR(100) NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
