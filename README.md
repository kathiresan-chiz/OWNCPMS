# College Placement Management System

## Introduction
The **College Placement Management System** is a web application designed to streamline and digitize the placement process in colleges and universities. The system features a multi-role platform catering to students, management, and super admin. It aims to minimize manual efforts, improve transparency, and provide real-time tracking of the placement cycle.

## Features
- **Student Portal**: Register and login, update profile, upload resume, view available job opportunities, apply for jobs, and track application status.
- **Management Admin Portal**: Access analytics, monitor placement stats, and view comprehensive reports.
- **Super Admin Portal**: Full control of the system including onboarding TPOs and management users, managing system configurations.
- **Cloudinary Integration**: Handles secure storage of profile pictures, resumes, and offer letters.

## Tech Stack
- **Frontend**: Vite + React.js, Tailwind CSS, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **File Storage**: Cloudinary
- **Styling**: Tailwind CSS, Bootstrap

## Project Structure
```plaintext
├── frontend
│   ├── public
│   ├── src
│   │   ├── api
│   │   ├── assets
│   │   ├── components
│   │   │   ├── LandingPages
│   │   │   └── students
│   │   ├── context
│   │   ├── hooks
│   │   ├── pages
│   │   ├── styles
│   │   ├── utility
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── .env (NOTE: YOU NEED TO CREATE THIS FILE)
│   ├── .gitignore
│   ├── .eslint.config.js
│   ├── index.html
│   ├── package-lock.json
│   ├── package.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   └── vite.config.js
├── backend
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── .env (NOTE: YOU NEED TO CREATE THIS FILE)
│   ├── .gitignore
│   ├── index.js
│   ├── package.json
│   └── package-lock.json
└── README.md
```

## User Roles
- **Students**: View and apply for jobs, update profile, track status, and upload resumes.
- **Management Admin**: Access dashboards and reports for data-driven decision making.
- **Super Admin**: Manage system settings, and create/manage TPO and Management users.

## Installation

### Prerequisites
- Node.js and npm installed
- MongoDB installed and running
- Cloudinary account for file uploads

### Clone the Repository
```bash
git clone https://github.com/kathiresan-chiz/OWNCPMS.git
```

### Backend Setup
1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```
2. Install the necessary packages:
   ```bash
   npm install
   ```
3. Create a `.env` file for environment variables:
   ```env
   PORT=4518
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   SMTP_USER="your_email_id"
   SMTP_PASS="your_app_password_to_be_generate_via_google_settings"
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `frontend` folder:
   ```bash
   cd frontend
   ```
2. Install the necessary packages:
   ```bash
   npm install
   ```
3. Create a `.env` file for environment variables:
   ```env
   VITE_BACKEND_URL=http://localhost:4518
   ```
4. Start the frontend development server:
   ```bash
   npm run dev
   ```


