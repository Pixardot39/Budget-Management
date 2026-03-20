# Budget Management System

A web-based budget management application that allows users to track and manage their personal incomes and expenses. Built as the final project for **CSE470 - Software Engineering** at BRAC University.

Live deployment: [https://budget-management-s5yw.onrender.com](https://budget-management-s5yw.onrender.com)

---

## Course Information

| Field        | Details                        |
|--------------|--------------------------------|
| Course Code  | CSE470                         |
| Course Name  | Software Engineering           |
| Group        | Group 4                        |
| Members      | Mashrafi, Ismaeel, Mahajabin, Esha |

---

## Overview

The Budget Management System is an online platform that provides users with a structured way to record, monitor, and analyze their financial activities. Users can log income and expense transactions, view summaries of their financial state, and receive automated notifications, all through a clean and responsive web interface.

This project was developed by a team of four members, all at the beginner level in web development. It represents a hands-on learning experience in applying software engineering principles — including requirements gathering, system design, team collaboration, and deployment — to build a fully functional application from scratch.

---

## Features

- User registration and login with secure password hashing
- Session-based authentication with JWT support
- Add, view, and manage income and expense records
- Dashboard with financial summaries
- Automated scheduled tasks using cron jobs
- Email notifications via Nodemailer
- Input validation for data integrity
- Responsive UI built with Bootstrap 5

---

## Tech Stack

### Backend
- **Runtime:** Node.js (v20.17.0)
- **Framework:** Express.js
- **Database:** MongoDB (via Mongoose)
- **Authentication:** bcrypt, JSON Web Tokens (jsonwebtoken), express-session, cookie-parser
- **Email:** Nodemailer
- **Scheduler:** node-cron
- **Validation:** validator
- **Other:** dotenv, method-override, axios

### Frontend
- **Templating Engine:** EJS with ejs-mate
- **Styling:** Bootstrap 5, CSS

### Dev Tools
- **Hot Reload:** nodemon

---

## Project Structure

```
Budget-Management/
├── middlewares/       # Custom middleware (auth checks, etc.)
├── models/            # Mongoose data models
├── public/            # Static assets (CSS, JS, images)
├── routes/            # Express route handlers
├── utils/             # Utility/helper functions
├── views/             # EJS templates
├── app.js             # Application entry point
├── package.json
└── .gitignore
```

---

## Getting Started

### Prerequisites

- Node.js v20.17.0 or higher
- MongoDB instance (local or cloud, e.g. MongoDB Atlas)
- npm

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mafimashrafi/Budget-Management.git
   cd Budget-Management
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and configure the following environment variables:

   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   SESSION_SECRET=your_session_secret
   EMAIL_USER=your_email_address
   EMAIL_PASS=your_email_password
   PORT=3000
   ```

4. Start the development server:

   ```bash
   npx nodemon app.js
   ```

   Or run without nodemon:

   ```bash
   node app.js
   ```

5. Open your browser and navigate to `http://localhost:3000`.

---

## Deployment

This application is deployed on [Render](https://render.com) and is publicly accessible at:

[https://budget-management-s5yw.onrender.com](https://budget-management-s5yw.onrender.com)

Note: As this is hosted on Render's free tier, the server may take a short moment to spin up on the first request after a period of inactivity.

---

## License

This project is licensed under the ISC License.
