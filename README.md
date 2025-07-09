# Final-Secure-Blog-System
This is the final project of my 45-day internship at ApexPlanet Software Pvt. Ltd. The project is a fully-functional secure blog web app built using PHP & MySQL. It integrates all the features from previous tasks into one final product.

## 🚀 Features Included
- CRUD (Create, Read, Update, Delete) Operations
- Secure User Login and Registration (password hashing, sessions)
- Role-based Access (Admin, Editor)
- Search functionality (by title or content)
- Pagination for better navigation
- Server and Client-side Form Validation
- PDO-based prepared statements for SQL security

## 📊 Technologies Used
- PHP
- MySQL
- HTML/CSS
- JavaScript (basic validation)
- XAMPP/WAMP
- Git & GitHub

## 🔄 User Roles
- **Admin**: Can create, edit, delete posts
- **Editor**: Can create and edit only

## 📚 DB Schema
```sql
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(255),
  password VARCHAR(255),
  role VARCHAR(50) DEFAULT 'editor'
);
CREATE TABLE posts (
  id INT AUTO_INCREMENT PRIMARY KEY,
  title VARCHAR(255),
  content TEXT,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
