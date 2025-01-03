
# Task Manager

## Overview
The **Task Manager** is a comprehensive application designed to streamline task and user management. It allows users to manage tasks, subtasks, and user roles efficiently with features like notifications, detailed task views, and analytics.

## Features
- **User Authentication:** Secure login system for users.
- **Task Management:** Create, update, and delete tasks and subtasks.
- **User Management:** Add, view, and manage user details.
- **Notifications:** Panel to keep track of updates.
- **Data Visualization:** Charts to analyze task progress and user activity.
- **Responsive Design:** Intuitive and responsive user interface built with TailwindCSS and React.
- **API-Driven Backend:** RESTful APIs for seamless communication between frontend and backend.

## Repository Content

### Client (Frontend)
The frontend is built using React and TailwindCSS.
- **Key Files/Folders:**
  - `components/`: Contains reusable UI components such as `TaskCard`, `Sidebar`, and `Navbar`.
  - `pages/`: Includes main pages like `Login`, `Tasks`, `Users`, and `Trash`.
  - `redux/`: State management using Redux Toolkit with slices for API and authentication.
  - `App.jsx`: Entry point for React app structure.
  - `vite.config.js`: Configuration file for Vite build tool.

### Server (Backend)
The backend is implemented using Node.js and Express.js.
- **Key Files/Folders:**
  - `controllers/`: Task and user logic in `taskController.js` and `userController.js`.
  - `middlewares/`: Handles authentication (`authMiddleware.js`) and errors (`errorMiddlewares.js`).
  - `models/`: MongoDB models for `task`, `user`, and `notification`.
  - `routes/`: API routes for tasks (`taskRoutes.js`) and users (`userRoutes.js`).
  - `utils/`: Utility functions for server-side operations.

### Other Key Files
- **Root Files:**
  - `index.html`: Entry point for the frontend application.
  - `package.json`: Contains dependencies and scripts for both client and server.
  - `tailwind.config.js`: TailwindCSS configuration.

## Installation and Setup

### Prerequisites
- **Node.js** and **npm** installed on your system.
- MongoDB database for backend integration.

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/ReetikaChavan/Task-Manager.git
   cd Task-Manager

2. **Install dependencies:**

For the client:
 ```bash
cd client
npm install
```
For the server:
 ```bash
cd server
npm install
```

3. **Set up the backend:**
1. **Configure environment variables in a .env file:**
MONGO_URI=<Your MongoDB URI>
JWT_SECRET=<Your JWT Secret>
Start the server:
 ```bash
npm start
```
Run the frontend:
 ```bash
cd client
npm run dev
```
Access the application: Open http://localhost:3000 in your browser.

**Key Functionalities**

1. Task Management: 
- Create, assign, and track tasks with deadlines.
- Subtask management for granular tracking.

2. User Management
- Add users and assign roles.
- View user-specific tasks and performance metrics.

3. Analytics and Reports
- Visualize task progress and user activity using charts.

4. Real-time Notifications
- Alerts for task updates and new assignments.


