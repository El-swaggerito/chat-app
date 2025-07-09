# Chat App

This is a full-stack chat application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) and Socket.io for real-time communication.

## Features

- User authentication (signup and login)
- Real-time messaging with Socket.io
- View online users
- Clean and responsive user interface

## Technologies Used

### Backend

- Node.js
- Express.js
- MongoDB
- Socket.io
- bcryptjs (for password hashing)
- JSON Web Tokens (for authentication)
- Mongoose (for MongoDB object modeling)

### Frontend

- React.js
- Zustand (for state management)
- Socket.io-client
- React Router DOM (for navigation)
- Tailwind CSS (for styling)
- DaisyUI (for UI components)

## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/chat-app.git
   cd chat-app
   ```

2. **Install backend dependencies:**
   ```bash
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   npm install --prefix frontend
   ```

4. **Create a `.env` file in the `backend` directory with the following environment variables:**
   ```
   PORT=<your_port_number>
   MONGO_DB_URI=<your_mongodb_connection_string>
   JWT_SECRET=<your_jwt_secret>
   NODE_ENV=<development_or_production>
   ```

5. **Build the frontend:**
   ```bash
   npm run build --prefix frontend
   ```

## Available Scripts

### In the root directory:

- `npm start`: Starts the backend server.
- `npm run server`: Starts the backend server using `nodemon` for development (auto-reloads on file changes).
- `npm run build`: Installs dependencies for both backend and frontend, and then builds the frontend.

### In the `frontend` directory:

- `npm run dev`: Starts the frontend development server (Vite).
- `npm run build`: Builds the frontend for production.
- `npm run lint`: Lints the frontend code.
- `npm run preview`: Serves the production build of the frontend locally.

## Project Structure

```
chat-app/
├── backend/                # Backend Node.js/Express.js application
│   ├── controllers/        # Request handlers
│   ├── db/                 # MongoDB connection logic
│   ├── middleware/         # Express middleware
│   ├── models/             # Mongoose models
│   ├── routes/             # API routes
│   ├── socket/             # Socket.io logic
│   ├── utils/              # Utility functions
│   └── server.js           # Main backend server file
├── frontend/               # Frontend React application
│   ├── public/             # Static assets
│   ├── src/                # Frontend source code
│   │   ├── assets/
│   │   ├── components/     # Reusable UI components
│   │   ├── context/        # React context providers
│   │   ├── hooks/          # Custom React hooks
│   │   ├── pages/          # Page components
│   │   ├── utils/          # Frontend utility functions
│   │   └── zustand/        # Zustand store for state management
│   ├── .eslintrc.cjs
│   ├── index.html
│   ├── package.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   └── vite.config.js
├── .gitignore
├── package.json            # Root package.json for backend and build scripts
└── README.md
```
