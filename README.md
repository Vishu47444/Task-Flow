A full-stack task management application built using MongoDB, Express.js, React, and Node.js (MERN). This app allows users to create, read, update, and delete tasks, providing a seamless experience for managing daily activities.

🛠️ Project Setup
Prerequisites
Ensure you have the following installed:

Node.js (v14 or higher)

MongoDB (local or MongoDB Atlas)

pnpm (recommended for package management)

1. Clone the Repository

git clone https://github.com/Vishu47444/Task-Flow

2. Install Dependencies
Install both frontend and backend dependencies using pnpm:

pnpm install-all
This command installs dependencies for both the frontend and backend.

3. Configure Environment Variables
Create a .env file in the backend directory with the following content:


PORT=5000
MONGO_URI=mongodb://localhost:27017/tasks  # Update with your MongoDB URI
JWT_SECRET=your_jwt_secret                 # Replace with your secret key
Ensure to replace MONGO_URI with your actual MongoDB connection string and JWT_SECRET with a strong secret key.

4. Start MongoDB
If you're using a local MongoDB instance, start it by running:

mongod
Alternatively, if you're using MongoDB Atlas, ensure your cluster is running and accessible.

5. Run the Application
To start both the frontend and backend servers concurrently, run:


pnpm run dev
This will start the backend on port 5000 and the frontend on port 3000. The app will automatically open in your default browser at http://localhost:3000.

🧠 Approach & Architecture
Backend (Server)
Express.js: Handles HTTP requests and routes.

MongoDB & Mongoose: Manages data storage and schema definitions.

JWT Authentication: Secures API endpoints and manages user sessions.

CORS: Configured to allow cross-origin requests from the frontend.

Frontend (Client)
React.js: Builds the user interface with component-based architecture.

React Router: Manages navigation between different views.

Axios: Facilitates HTTP requests to the backend API.

lucide-react : Provides pre-designed components for a responsive UI.

Features
User authentication (register, login, logout)

CRUD operations for tasks

Task categorization (e.g., To-Do, In Progress, Completed)

Responsive design for mobile and desktop views

⚠️ Assumptions & Trade-offs
Assumptions
Users have basic knowledge of using web applications.

The application is intended for personal or small team use.

MongoDB is used for data storage; no SQL database is involved.

Trade-offs
No Role-Based Access Control (RBAC): The app assumes all users have the same level of access, which may not be suitable for larger teams requiring different permission levels.

No Real-Time Updates: The application does not implement real-time features like WebSockets, so users need to refresh the page to see updates made by others.
