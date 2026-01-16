# Book Store - MERN Stack Application

A full-stack expense tracking application built with MongoDB, Express.js, React, and Node.js. Track your income and expenses with an intuitive dashboard, charts, and transaction management.

## Features

- 🔐 User Authentication (Register/Login)
- 💰 Income Management (Add, View, Delete)
- 📊 Dashboard with Summary Cards

### Frontend
- React 18.2.0
- React Router DOM
- Axios
- Recharts (for data visualization)
- React Icons

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- bcryptjs (password hashing)

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local installation or MongoDB Atlas account)

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ETS-MERN.git
cd ETS-MERN
```

### 2. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory:

```env
MONGODB_URI=mongodb://localhost:27017/expense-tracker
PORT=5000
JWT_SECRET=your-super-secret-jwt-key-change-this-in-production
```

**Important:** Generate a strong random string for `JWT_SECRET` in production. You can use:
```bash
node -e "console.log(require('crypto').randomBytes(32).toString('hex'))"
```

### 3. Frontend Setup

```bash
cd ../frontend
npm install
```

Create a `.env` file in the `frontend` directory:

```env
REACT_APP_API_URL=http://localhost:5000
```

For production, update this to your backend URL:
```env
REACT_APP_API_URL=https://your-backend-domain.com
```

## Running the Application

### Development Mode

1. **Start MongoDB** (if using local installation):
   ```bash
   mongod
   ```

2. **Start the Backend Server**:
   ```bash
   cd backend
   npm start
   # or for development with auto-reload:
   npm run dev
   ```
   The backend will run on `http://localhost:5000`

3. **Start the Frontend** (in a new terminal):
   ```bash
   cd frontend
   npm start
   ```
   The frontend will run on `http://localhost:3000`

4. Open your browser and navigate to `http://localhost:3000`


