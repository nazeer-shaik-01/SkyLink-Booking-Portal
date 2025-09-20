
# ✈️ AeroGrid - Full-Stack Airline Reservation System

AeroGrid is a complete, full-stack web application for booking and managing flights, built with a **Spring Boot backend** and an **Angular frontend**.
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

### 🔐 Authentication

![Login & Register](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Login.png)

### 🛫 Airports Management

![Airports CRUD](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Airports.png)

### ✈️ Aircraft Management

![Aircraft CRUD](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Aircraft.png)

### 🗓️ Schedule Flights

![Schedule Flight](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Schedule_flight.png)

### 🔍 Search Flights

![Flight Search](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Search.png)

### 🎟️ My Bookings

![Bookings](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Bookings.png)

---


👉 Do you want me to also write a **step-by-step Setup Guide** (clone, backend run, frontend run) section for the README so others can run it easily?
