# Todo App

## Description

This Todo App is a simple web application that allows users to manage their daily tasks. It provides functionalities to add, edit, and delete tasks, along with the option to mark tasks as completed. The application has a frontend built with **React** and **Vite**, while the backend is developed with **Node.js** and **Express**. Data is stored in **MongoDB**, and user authentication is handled using **Passport.js**.

## Project Structure

The project is divided into two main components:

1. **Frontend** (Located in `/todo-app`): This contains all the client-side code for the React app.
2. **Backend** (Located in `/server`): This contains the server-side logic, including API routes and database handling.

```
TODO APP/
├── node_modules/
├── server/
│   ├── models/
│   ├── routes/
│   ├── app.js
│   ├── package.json
├── todo-app/
│   ├── src/
│   ├── dist/
│   ├── public/
│   ├── package.json
├── README.md
```

## Setup Instructions

### Prerequisites

- Node.js (v18 or later)
- MongoDB (Running locally or using MongoDB Atlas)
- Docker (optional, for containerized environment)

### Running the App Locally

#### 1. Clone the repository

```bash
git clone https://github.com/your-repo/todo-app.git
cd todo-app
```

#### 2. Install dependencies

**Frontend:**

```bash
cd todo-app
npm install
```

**Backend:**

```bash
cd ../server
npm install
```

#### 3. Set up environment variables

In the backend (`/server`), create a `.env` file and add your MongoDB connection string, along with any other environment variables needed (e.g., `PORT`, `JWT_SECRET`).

Example `.env` file:

```
MONGODB_URI=mongodb://localhost:27017/todoapp
JWT_SECRET=your_secret_key
```

#### 4. Start the application

**Frontend:**

```bash
cd todo-app
npm run dev
```

**Backend:**

```bash
cd ../server
npm start
```

You should now have both the frontend and backend running. The frontend is served at `http://localhost:5173`, and the backend API at `http://localhost:3000`.

## Technologies Used

- **Frontend**: React, Vite, Tailwind CSS
- **Backend**: Node.js, Express, Passport.js for authentication
- **Database**: MongoDB
- **Containerization**: Docker, Docker Compose
- **Authentication**: Passport.js with Local Strategy

## Features

- User Authentication (Login/Signup)
- Add, Edit, and Delete tasks
- Mark tasks as completed
- Responsive design

## Future Improvements

- Add filtering and sorting options for tasks
- Improve authentication with OAuth providers (Google, Facebook, etc.)
- Add real-time features with WebSockets

## License

This project is licensed under the MIT License.
