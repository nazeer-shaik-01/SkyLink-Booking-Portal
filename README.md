
# ✈️ SkyLink-Booking-Portal - Full-Stack Airline Reservation System

SkyLink-Booking-Portal is a complete, full-stack web application for booking and managing flights, built with a **Spring Boot backend** and an **Angular frontend**.
It features a secure, role-based system that provides distinct interfaces for **public users** and **administrators**.

---

## ✨ Features

### 👨‍✈️ Admin Panel

* Full **CRUD (Create, Read, Update, Delete)** management for:

  * Airports
  * Aircraft
  * Flights

### 🧑‍💻 User Interface

* Publicly accessible **flight search** (by source, destination, and date).
* Secure **flight booking** for authenticated users.
* A **My Bookings** page to view user flight history.

### 🔒 Security

* User registration and login system.
* Role-based access control (`USER` vs. `ADMIN`).
* Secure APIs using **Spring Security** and **JSON Web Tokens (JWT)**.

---

## 🛠️ Technology Stack

### Backend

* Java & Spring Boot
* Spring Security + JWT (authentication & authorization)
* Spring Data JPA + Hibernate
* MySQL Database

### Frontend

* Angular + TypeScript
* Angular CLI
* HTML + CSS

---

## 🗃️ Database Schema

The application uses a relational database with the following **core entities**:

* **User:** Stores user credentials and roles.
* **Role:** Defines permissions (`ROLE_USER`, `ROLE_ADMIN`).
* **Airport:** Airport details (code, name, city, country).
* **Aircraft:** Aircraft details (model, capacity).
* **Flight:** Links source airport, destination airport, and aircraft.
* **Booking:** Connects a user to a flight.

---

## 🔌 API Endpoints

### 🔑 Authentication API

* `POST /api/auth/register` → Register a new user.
* `POST /api/auth/login` → Authenticate and receive JWT.

### 🌍 Public API

* `GET /api/flights/search` → Search available flights.
* `GET /api/flights/airports` → Fetch all airports.

### 👤 User API (Requires `ROLE_USER`)

* `POST /api/bookings` → Create a new booking.
* `GET /api/bookings/my` → Get logged-in user’s bookings.

### 🛠️ Admin API (Requires `ROLE_ADMIN`)

* `GET | POST | PUT | DELETE /api/admin/airports/**`
* `GET | POST | PUT | DELETE /api/admin/aircrafts/**`
* `GET | POST | PUT | DELETE /api/flights/admin/**`

---

## 📸 Screenshots

### 📝 Register

![Register](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Register_page.png)

### 🔐 Login

![Login](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Login_page.png)

### 🛫 Manage Airports

![Airports](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Manage_airport.png)

### ✈️ Manage Aircraft

![Aircraft](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Manage_aircraft.png)

### 🗓️ Schedule Flights

![Schedule Flights](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Schedule_flight.png)

### 🔍 Search Flights

![Search Flights](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/Search_flight.png)

### 🎟️ My Bookings

![Bookings](https://raw.githubusercontent.com/nazeer-shaik-01/SkyLink-Booking-Portal/main/airline-frontend/airline-frontend/pics/My_bookings.png)

---
