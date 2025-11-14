# Bus Booking System

A full-stack bus booking system built with a React frontend, Node.js/Express backend, and MySQL database **SERN stack**. This platform offers complete functionality for both admin and user roles, enabling efficient bus management, route scheduling, seat booking, and payment tracking.

---

## 🚀 Features

### Admin Interface
- Manage buses: add, update, or delete bus details.
- Configure and manage bus schedules.
- Create and manage routes, stops, and route variants (for different paths or timings).
- Manage admins: add new admin accounts and fetch all existing admins.
- View complete payment history and analyze total earnings.

### User Interface
- Sign up, log in, and log out functionality.
- Search available buses between selected source and destination.
- View detailed bus schedules and seat availability.
- Book seats and view booking history (upcoming and past trips).
- Update personal profile information easily.

---

## 🧩 Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend | React, Zustand (for state management), Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MySQL (nested queries, functions, procedures, triggers) |
| Authentication | JWT (JSON Web Tokens) |
| API | Axios |
| Notifications | React Hot Toast |

---

## ⚙️ Installation and Setup

Follow these steps to set up the development environment:

### 1. Clone the Repository
```bash
git clone https://github.com/Dhruthi-Kedilaya/bus-booking-app.git
cd bus-booking-app
```
## 🔐 Environment Variables
Create a `.env` file inside the backend directory (see environment configuration below).  
Then start the backend server:
```bash
PORT=3000 # Backend server port
DB_HOST=localhost # Database host
DB_USER=root # MySQL username
DB_PASSWORD= # MySQL password
DB_NAME=citizen_portal # Database name
DB_PORT=3306 # MySQL port (default: 3306)
JWT_SECRET=your_secret_key # Secret key for JWT authentication
NODE_ENV=development # Environment mode (development/production)
```
### 2. Backend Setup
```bash
cd backend
npm install
nodemon src/index.js
```

### 3. Frontend Setup(in new terminal)
```bash
cd /frontend
npm install
npm run dev
```

---

## 🗄️ Database Structure

This project uses a relational MySQL database with tables for:
- Citizens  
- Admin 
- Bus
- Bus_stops
- Busschedule 
- Routes
- RouteStops
- RouteVariants 
- Booking 
- Payment 

The schema file `database/structure.sql` defines all tables and relationships required for initializing the database citizen_portal.

---

## 💡 Key Implementation Notes

- State management is handled using **Zustand**, ensuring lightweight and efficient state synchronization.
- Authentication uses **JWT tokens**, stored securely in local storage.
- Backend APIs follow RESTful design principles.
- Error handling and toast notifications enhance the user experience.
- Environment-specific configuration enables flexible deployment.
- Database is efficiently designed with triggers, stored procedures, functions, nested queries, and transaction-based operations for maintaining data integrity and optimizing performance.





