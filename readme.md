# Eventora 🎟️

A full-stack event booking and management platform built with the MERN stack. Eventora enables users to discover events, securely book tickets through OTP verification, and track their bookings, while administrators can manage events, review booking requests, monitor revenue, and oversee platform activity through a dedicated dashboard.

## 🚀 Features

### 🔐 Authentication & Security

* Secure user registration and login using JWT Authentication and bcrypt password hashing.
* Email-based OTP verification for account activation.
* Protected routes and role-based authorization.
* Secure booking verification through OTP confirmation.

### 👥 Role-Based Access Control

#### Admin

* Create, update, and delete events.
* Manage free and paid events.
* Review booking requests.
* Approve or reject bookings.
* Mark bookings as paid or unpaid.
* Access platform analytics and booking statistics.

#### User

* Browse available events.
* View detailed event information.
* Book tickets using OTP verification.
* Track booking status through a personal dashboard.
* Cancel pending bookings.

### 🎫 Event Management

* Create free and paid events.
* Add event descriptions, categories, dates, venue details, and event images.
* Configure seating capacity for each event.
* Real-time seat availability tracking.

### 📩 Smart Booking Workflow

* OTP-protected booking requests.
* Pending booking approval system.
* Overbooking prevention through seat validation.
* Automated booking confirmation emails.
* Booking cancellation support.

### 📊 Admin Analytics Dashboard

* Total events overview.
* Pending booking requests.
* Confirmed bookings statistics.
* Revenue tracking for paid events.
* User and booking activity insights.

### 📧 Email Notifications

* Account verification emails.
* Booking OTP delivery.
* Booking confirmation notifications.
* Status update emails using Nodemailer.

### 🎨 Modern User Interface

* Responsive design for desktop and mobile devices.
* Built using React and Tailwind CSS.
* Clean and intuitive user experience.
* Smooth interactions and user-friendly workflows.

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Tailwind CSS
* Axios
* React Router DOM

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### Authentication & Security

* JWT (JSON Web Tokens)
* bcrypt

### Email Services

* Nodemailer

### Database

* MongoDB Atlas

---

## 📂 Project Structure

```text
Eventora/
│
├── client/                 # React Frontend
│   ├── src/
│   ├── public/
│   └── package.json
│
├── server/                 # Express Backend
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   └── package.json
│
├── package.json
└── README.md
```

---

## ⚙️ Environment Variables

Create a `.env` file inside the `server` directory and add the following variables:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
EMAIL_USER=your_email_address
EMAIL_PASS=your_email_app_password
PORT=5000
```

> Note: For Gmail, use an App Password instead of your regular account password.

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
cd Eventora
```

### 2. Install Dependencies

Install all project dependencies:

```bash
npm install
npm run install:all
```

---

## ▶️ Run the Application

### Start Frontend and Backend Together

```bash
npm run dev
```

### Or Run Separately

#### Backend

```bash
cd server
npm install
npm run dev
```

Backend runs on:

```text
http://localhost:5000
```

#### Frontend

```bash
cd client
npm install
npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

---

## 🔄 Booking Flow

```text
User Registration
        ↓
Email OTP Verification
        ↓
Browse Events
        ↓
Book Event
        ↓
Booking OTP Verification
        ↓
Pending Approval
        ↓
Admin Review
        ↓
Booking Confirmed
        ↓
Email Notification Sent
```

---

## 📈 Key Functionalities

* JWT Authentication
* OTP Verification System
* Role-Based Authorization
* Event Management
* Seat Capacity Validation
* Booking Approval Workflow
* Revenue Tracking
* Email Notifications
* Admin Dashboard Analytics
* Responsive UI

---

## 🎯 Learning Outcomes

This project demonstrates practical experience with:

* Full-Stack MERN Development
* REST API Design
* Authentication & Authorization
* MongoDB Database Modeling
* OTP-Based Verification Systems
* Email Service Integration
* State Management
* Backend Business Logic
* Admin Dashboard Development
* Secure Booking Workflows

---

## 👨‍💻 Author

Developed as a full-stack MERN application to explore authentication, event management, booking workflows, and dashboard analytics in a real-world business use case.
