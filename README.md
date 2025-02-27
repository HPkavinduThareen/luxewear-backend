# Backend Project - Crop Monitoring System

## Description
This is the backend for the **Crop Monitoring System**, built using **Node.js, Express, MongoDB, and JWT authentication**. It provides a REST API for managing crops, fields, staff, equipment, and monitoring logs. The system ensures secure authentication and authorization using JWT.

---

## Features
- **Authentication & Authorization**: Secure user login and registration with JWT.
- **CRUD Operations**: Manage crops, fields, staff, and equipment.
- **MongoDB Integration**: Data storage with Mongoose ORM.
- **Middleware**: Authentication and error handling.
- **REST API**: Endpoints for handling crop management tasks.
- **Express.js Server**: Fast and lightweight backend framework.

---

## Technologies Used
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web framework for Node.js
- **MongoDB** - NoSQL database for storing data
- **Mongoose** - ODM (Object Data Modeling) library for MongoDB
- **JWT (JSON Web Token)** - Authentication mechanism
- **Bcrypt.js** - Password hashing
- **Cors** - Cross-Origin Resource Sharing
- **Dotenv** - Environment variable management

---

## Installation Guide

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v14 or later)
- **MongoDB** (running locally or a cloud database like MongoDB Atlas)
- **Git**

### Clone the Repository
```sh
git clone https://github.com/your-username/crop-monitoring-backend.git
cd crop-monitoring-backend
```

### Install Dependencies
```sh
npm install
```

### Set Up Environment Variables
Create a `.env` file in the root directory and add the following:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Start the Server
```sh
npm start
```

The server will run on `http://localhost:5000`

---

## API Endpoints
### Authentication
- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - User login
- **POST** `/api/auth/refresh` - Refresh JWT token

### Crop Management
- **GET** `/api/crops` - Get all crops
- **POST** `/api/crops` - Add a new crop
- **PUT** `/api/crops/:id` - Update crop details
- **DELETE** `/api/crops/:id` - Delete a crop

### Field Management
- **GET** `/api/fields` - Get all fields
- **POST** `/api/fields` - Add a new field
- **PUT** `/api/fields/:id` - Update field details
- **DELETE** `/api/fields/:id` - Delete a field

---

## Project Structure
```
backend/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── server.js
├── .env
├── .gitignore
├── package.json
├── README.md
```

---

## Deployment
### Deploy to Heroku
```sh
git push heroku main
```

### Deploy to Vercel
```sh
vercel --prod
```

---

## License
This project is licensed under the MIT License.

---

## Contributors
- Your Name (@your-github-handle)

Feel free to contribute by submitting issues or pull requests!

---

