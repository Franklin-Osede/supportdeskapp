# Support Desk App

## About the Project

The **Support Desk App** is a full-stack application built using the **MERN stack** (MongoDB, Express.js, React, and Node.js). It enables users to create support tickets, manage issues, and track the status of their tickets efficiently. The app provides both a user-friendly frontend and a robust backend to manage support operations seamlessly.

---

## Features

- **User Authentication**:
  - Register, login, and manage sessions securely.
- **Ticket Management**:
  - Create, view, update, and delete support tickets.
  - Track ticket status (e.g., Open, In Progress, Resolved).
- **Admin Dashboard**:
  - Manage user accounts and oversee all tickets.
- **Real-Time Updates**:
  - Dynamic frontend updates using React hooks.
- **Responsive Design**:
  - Optimized for mobile, tablet, and desktop views.

---

## Project Structure

### Frontend

Located in the `frontend/` folder, the frontend is built with **React** and includes:

- **`app/`**: Contains global state and application-level configuration.
- **`components/`**: Reusable UI components, such as forms, buttons, and modals.
- **`features/`**: Implements features like ticket creation and user profile management.
- **`hooks/`**: Custom React hooks for managing state and side effects.
- **`pages/`**: Pages for the app, including Login, Dashboard, and Ticket Details.
- **`App.js`**: Root component that handles routing.
- **`index.js`**: Entry point for the React app.

### Backend

Located in the `backend/` folder, the backend is built with **Node.js** and **Express.js** and includes:

- **`config/`**: Contains configuration files (e.g., database connection).
- **`controllers/`**: Handles business logic for routes.
- **`middleware/`**: Custom middleware for authentication and error handling.
- **`models/`**: Mongoose schemas for MongoDB collections (e.g., Users, Tickets).
- **`routes/`**: API endpoints for user and ticket management.
- **`server.js`**: Main entry point for the backend application.

---

## Prerequisites

- **Node.js**: Ensure Node.js is installed on your system.
- **MongoDB**: Install and run a MongoDB instance locally or use a cloud service like MongoDB Atlas.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/support-desk-app.git
   cd support-desk-app
   ```

2. Install dependencies for both the frontend and backend:
   ```bash
   cd backend
   npm install
   cd ../frontend
   npm install
   ```

3. Set up environment variables:

   In the `backend` folder, create a `.env` file with the following:
   ```env
   NODE_ENV=development
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

---

## Running the Application

1. Start the backend server:
   ```bash
   cd backend
   npm run server
   ```

2. Start the frontend development server:
   ```bash
   cd frontend
   npm start
   ```

3. Open your browser and visit [http://localhost:3000](http://localhost:3000).

---

## API Endpoints

The backend provides the following API endpoints:

- **Authentication**:
  - `POST /api/users/register`: Register a new user.
  - `POST /api/users/login`: Authenticate a user and get a token.
- **Tickets**:
  - `GET /api/tickets`: Fetch all tickets for the logged-in user.
  - `POST /api/tickets`: Create a new support ticket.
  - `PUT /api/tickets/:id`: Update a ticket by ID.
  - `DELETE /api/tickets/:id`: Delete a ticket by ID.

---

## Built With

- **MongoDB**: Database for storing user and ticket data.
- **Express.js**: Backend framework for building APIs.
- **React**: Frontend library for building user interfaces.
- **Node.js**: JavaScript runtime for backend development.
- **JWT**: For secure authentication.

---

## Contributing

Contributions are welcome! Follow these steps to contribute:

1. Fork the project.
2. Create your feature branch:
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

## Project Link

[GitHub Repository](https://github.com/yourusername/support-desk-app)

---

This README provides a comprehensive overview of the Support Desk App, including its features, structure, and instructions for setting up and running the project. If you have any questions or suggestions, feel free to contribute or open an issue!
