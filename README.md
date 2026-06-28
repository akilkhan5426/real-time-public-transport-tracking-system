# 🚍 Real-Time Public Transport Tracking System

A full-stack mobile application that enables commuters to track public transport buses in real time using GPS. The system provides live bus locations on an interactive map through WebSockets while exposing REST APIs for authentication, trip management, and transport services.

---

## 📖 Overview

The Real-Time Public Transport Tracking System is designed to improve the public transportation experience by allowing passengers to monitor the live location of buses from their mobile devices. The application combines GPS tracking, WebSockets, REST APIs, and Google Maps to deliver low-latency location updates.

The backend follows a scalable Node.js and Express architecture with MongoDB as the primary database and JWT-based authentication for secure access.

---

## ✨ Features

### Passenger Features

* View active buses
* Live GPS tracking on Google Maps
* Search available routes
* View bus details
* Receive real-time location updates

### Driver Features

* Secure login using JWT
* Start and stop trips
* Continuously publish GPS coordinates
* Automatic real-time location broadcasting

### Admin Features

* Manage buses
* Manage drivers
* Manage routes
* Monitor active trips
* Dashboard statistics

---

## 🛠 Tech Stack

### Frontend

* React Native

### Backend

* Node.js
* Express.js

### Database

* MongoDB (Mongoose)

### Real-Time Communication

* Socket.IO (WebSockets)

### APIs

* REST API
* Google Maps API

### Authentication

* JWT
* bcryptjs

### Other Libraries

* Helmet
* CORS
* Express Validator

---

## 🏗 System Architecture

```text
React Native App
        │
        ▼
REST APIs + WebSockets
        │
Node.js + Express Server
        │
 ┌──────────────┐
 │ MongoDB      │
 │ GPS Logs     │
 │ Trips        │
 │ Routes       │
 │ Buses        │
 │ Users        │
 └──────────────┘
```

---

## 🔄 Application Workflow

1. Driver logs into the application.
2. Driver starts a trip.
3. GPS coordinates are sent periodically to the backend.
4. The backend stores location updates in MongoDB.
5. Socket.IO broadcasts updated locations to subscribed users.
6. React Native displays live bus movement on Google Maps.

---

## 📂 Database Collections

* Users
* Buses
* Routes
* Stops
* Trips
* GPS Logs
* Stop Arrivals

---

## 🔌 REST APIs

The backend exposes REST APIs for:

* Authentication
* Route Management
* Bus Information
* Trip Management
* Driver Operations
* Admin Operations
* Live Bus Location

---

## ⚡ WebSocket Events

### Client → Server

* subscribe-bus
* unsubscribe-bus
* location-update

### Server → Client

* bus-location
* trip-status

---

## 📚 Learning Outcomes

* Built a scalable RESTful backend using Express.js.
* Integrated MongoDB using Mongoose.
* Implemented JWT-based authentication and role-based authorization.
* Used Socket.IO for real-time GPS tracking.
* Integrated Google Maps API with React Native.
* Designed REST APIs following a modular architecture.
* Worked collaboratively using Git and GitHub.

---

## 🚀 Future Enhancements

* ETA prediction using Machine Learning
* Push notifications
* Offline GPS synchronization
* Multi-city deployment
* Cloud deployment on AWS
* Route analytics dashboard

---

## 👥 Team

**Team Size:** 3

---

## 📄 License

This project was developed for academic and learning purposes.
