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
* A **My Bookings** page to view flight history.

### 🔒 Security

* User registration and login system.
* Role-based access control (`USER` vs. `ADMIN`).
* Secure APIs using **Spring Security** and **JSON Web Tokens (JWT)**.

---

## 🛠️ Technology Stack

### Backend

* Java & Spring Boot
* Spring Security + JWT
* Spring Data JPA + Hibernate
* MySQL Database

### Frontend

* Angular + TypeScript
* Angular CLI
* HTML + CSS

---

## 🗃️ Database Schema

The application uses the following **core entities**:

* **User** → Stores credentials and roles
* **Role** → Defines permissions (`ROLE_USER`, `ROLE_ADMIN`)
* **Airport** → Code, name, city, country
* **Aircraft** → Model and capacity
* **Flight** → Links source, destination, aircraft
* **Booking** → Connects a user to a flight

---

## 🔌 API Endpoints

### 🔑 Authentication API

* `POST /api/auth/register` → Register a new user
* `POST /api/auth/login` → Authenticate and receive JWT

### 🌍 Public API

* `GET /api/flights/search` → Search flights
* `GET /api/flights/airports` → List airports

### 👤 User API (Requires `ROLE_USER`)

* `POST /api/bookings` → Create booking
* `GET /api/bookings/my` → Get user’s bookings

### 🛠️ Admin API (Requires `ROLE_ADMIN`)

* `GET | POST | PUT | DELETE /api/admin/airports/**`
* `GET | POST | PUT | DELETE /api/admin/aircrafts/**`
* `GET | POST | PUT | DELETE /api/flights/admin/**`

---

## 📸 Screenshots

### 📝 Register

![Register](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/register.png)

### 🔐 Login

![Login](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/login.png)

### 🛫 Airport Management

![Airports](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/airport.png)

### ✈️ Aircraft Management

![Aircraft](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/aircraft.png)

### 🗓️ Flight Management

![Flight Management](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/Schedule_flight.png)

### 🔍 Flight Search

![Search Flights](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/search_flight.png)

### 🎟️ My Bookings

![Bookings](https://github.com/nazeer-shaik-01/SkyLink-Booking-Portal/blob/main/airline-frontend/airline-frontend/pics/bookings.png)

---
