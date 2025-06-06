A full-stack task management application built using MongoDB, Express.js, React, and Node.js (MERN). This app allows users to create, read, update, and delete tasks, providing a seamless experience for managing daily activities.

🛠️ Project Setup

SETUP INSTRUCTIONS

Backend Setup

Environment variables
   
First, create the environment variables file .env in the server folder. The .env file contains the following environment variables:

MONGODB_URI = your MongoDB URL

JWT_SECRET = any secret key - must be secured

PORT = 8800 or any port number 

NODE_ENV = development
 
Set Up MongoDB:

Setting up MongoDB involves a few steps:

1. Visit MongoDB Atlas Website

Go to the MongoDB Atlas website: https://www.mongodb.com/cloud/atlas.
Create an Account

Log in to your MongoDB Atlas account.

Create a New Cluster

Choose a Cloud Provider and Region

Configure Cluster Settings

Create Cluster

Wait for Cluster to Deploy

Create Database User

Set Up IP Whitelist

Connect to Cluster

Configure Your Application

Test the Connection

2. Create a new database and configure the .env file with the MongoDB connection URL.

   

Steps to run backend

1.Open the project in any editor of choice.

2.Navigate into the server directory cd backend.

3.Run npm i or npm install to install the packages.

4.Run npm start to start the server.

If configured correctly, you should see a message indicating that the server is running successfully and Database Connected.



 

Frontend Side Setup


Steps to run fontend

1. Navigate into the client directory cd frontend.

2. Run npm i or npm install to install the packages.

3. Run npm start to run the app on your local browser.









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









⚠️ Assumptions & Trade-offs

Assumptions


Users have basic knowledge of using web applications.

The application is intended for personal or small team use.

MongoDB is used for data storage; no SQL database is involved.



Trade-offs


No Role-Based Access Control (RBAC): The app assumes all users have the same level of access, which may not be suitable for larger teams requiring different permission levels.

No Real-Time Updates: The application does not implement real-time features like WebSockets, so users need to refresh the page to see updates made by others.
