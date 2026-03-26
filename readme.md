# Backend Ledger API

A **Node.js + Express + MongoDB** based backend system that simulates a **digital wallet / ledger system** similar to real-world financial applications like UPI or Paytm.

This project focuses on **account management, transactions, and secure authentication**, providing a scalable backend architecture.

---

## Features

- User Authentication (JWT-based)
- User Registration & Login
- Account Creation & Management
- Transaction Processing (Transfer money)
- Ledger-based balance tracking
- Token Blacklisting (Logout security)
- Error Handling & Validation
- Email Notifications (optional)

---

## Project Overview

This project simulates how financial systems work internally:

```text
User → Account → Transaction → Ledger Updates

---

## Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB (Mongoose)
* **Authentication:** JWT
* **Environment Config:** dotenv
* **Email Service:** Nodemailer
* **Other:** bcrypt, middleware, REST APIs

---

## Folder Structure

```
backend-ledger/
│── src/
│   ├── config/        # DB configuration
│   ├── controllers/   # Business logic
│   ├── models/        # Mongoose schemas
│   ├── routes/        # API routes
│   ├── middleware/    # Auth middleware
│   ├── services/      # Email service
│   └── app.js         # Main app
│
├── server.js          # Entry point
├── .env               # Environment variables
├── package.json
```

---

## API Endpoints

### Auth Routes

| Method | Endpoint             | Description   |
| ------ | -------------------- | ------------- |
| POST   | `/api/auth/register` | Register user |
| POST   | `/api/auth/login`    | Login user    |

---

### Account Routes

| Method | Endpoint       | Description         |
| ------ | -------------- | ------------------- |
| POST   | `/api/account` | Create account      |
| GET    | `/api/account` | Get account details |

---

### Transaction Routes

| Method | Endpoint           | Description      |
| ------ | ------------------ | ---------------- |
| POST   | `/api/transaction` | Transfer money   |
| GET    | `/api/transaction` | Get transactions |

---

## Testing

Use **Postman**

Example request:

```json
POST /api/auth/register
{
  "name": "Js",
  "email": "test@gmail.com",
  "password": "123456"
}
```

---

## Future Improvements

* Dashboard (Frontend)
* Payment Gateway Integration
* Analytics & Reports

---

## Show your support

If you like this project, give it a ⭐ on GitHub!

````