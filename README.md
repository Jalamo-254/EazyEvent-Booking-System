# EazyEvent-Booking-System
# 🎟️ EazyEvent Booking System

EazyEvent is a lightweight **PHP + MySQL Event Booking System** that allows users to browse and register for events, while admins can manage events and view bookings. Built with **PHP, HTML, CSS, and JavaScript**, this project is perfect for learning full-stack development and can evolve into a production-ready system.

---

## 🚀 Features

### User Side
- User Registration & Login (Session-based authentication)
- Browse upcoming events with details (title, date, time, venue, capacity)
- Book or cancel event registrations
- See **remaining slots** dynamically updated with JavaScript (AJAX)
- User Dashboard showing booked events

### Admin Side
- Secure Admin Login
- Add / Edit / Delete events
- Upload event images
- View all bookings for each event
- Dashboard stats (Users, Events, Bookings)

---

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3, JavaScript (with AJAX for dynamic updates)
- **Backend:** PHP 8+
- **Database:** MySQL
- **Styling:** Custom CSS (Bootstrap/Tailwind optional)
- **Charting (Optional):** Chart.js for analytics

---

## 📂 Project Structure

event_booking/
│
├── config/ # Database connection
├── admin/ # Admin panel (login, dashboard, manage events)
├── user/ # User panel (register, login, dashboard)
├── includes/ # Shared header, footer, navbar
├── assets/ # CSS, JS, images
└── index.php # Homepage (list of events)

yaml
Copy
Edit

---

## 🛢️ Database Schema

### users
- id (PK)
- name
- email
- password
- role (user/admin)
- created_at

### events
- id (PK)
- title
- description
- date
- time
- venue
- capacity
- slots_remaining
- image
- created_at

### bookings
- id (PK)
- user_id (FK → users.id)
- event_id (FK → events.id)
- booked_at

---

## ⚡ Setup Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/EazyEvent-Booking-System.git
Import the SQL file into your MySQL database:

sql
Copy
Edit
CREATE DATABASE eazyevent_db;
USE eazyevent_db;
-- import schema.sql
Update your /config/db.php with database credentials.

Run the project locally using XAMPP, WAMP, or Laragon:

arduino
Copy
Edit
http://localhost/event_booking/
🎯 Future Enhancements
Email notifications after booking

QR code ticket generation

Payment integration (M-PESA, PayPal)

Advanced analytics with charts

👨‍💻 Author
Jerry Ouma Otieno (Easytech Hub Solutions)
🔗 Portfolio Website
📧 easytechhubsolutions@gmail.com

⚠️ Disclaimer: This is a learning project intended for educational use. Not production-ready without additional security hardening.

pgsql
Copy
Edit

---

Do you want me to also draft the **SQL schema file (schema.sql)** so that when you clone and import, you’re instantly ready to go?








Ask ChatGPT
