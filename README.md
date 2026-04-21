# --ChatNow--

## 1.0 Project Overview
ChatNow is a full-stack, real-time messaging application built using the MERN stack. It allows users to create accounts, update their profiles, and engage in real-time text and media conversations with other registered users.

## 2.0 Key Features
* **Real-Time Messaging:** Instant message delivery and live updates.
    * *Example:* When User A types and sends "Hello," User B sees the message appear immediately on their screen without needing to refresh the page, powered by Socket.io web sockets.
* **User Authentication & Security:** Secure signup, login, and logout functionality.
    * *Example:* User passwords are encrypted before being saved to the database, and user sessions are securely managed using HTTP-only JSON Web Tokens (JWT).
* **Media Sharing:** Users can attach and send images within their conversations.
    * *Example:* A user can click the attachment icon, select a `.jpg` or `.png` file, and upload it. The image is hosted on Cloudinary and rendered instantly in the chat window.
* **Responsive UI:** A modern, clean interface that adapts to different devices.
    * *Example:* The layout gracefully shifts from a persistent side-by-side sidebar view on desktop to a compact, toggleable mobile-friendly view on smaller screens using Tailwind CSS and DaisyUI.

## 3.0 Tech Stack
* **Frontend:** React, Zustand (Global State Management), Tailwind CSS, DaisyUI, React Router.
* **Backend:** Node.js, Express.js, MongoDB (Mongoose), Socket.io (Real-time communication), Cloudinary (Image Hosting).

## 4.0 Setup and Installation
To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd ChatNow
    ```
2.  **Install dependencies:**
    The project contains a root `package.json` that can handle installations.
    ```bash
    npm run build
    ```
    *(Alternatively, navigate to both the `frontend/` and `backend/` directories and run `npm install` in each).*
3.  **Configure Environment Variables:**
    Create a `.env` file inside the `backend/` directory and add the following keys:
    ```env
    PORT=5001
    MONGODB_URI=your_mongodb_connection_string
    JWT_SECRET=your_secure_jwt_secret_key
    NODE_ENV=development
    CLOUDINARY_CLOUD_NAME=your_cloudinary_name
    CLOUDINARY_API_KEY=your_cloudinary_api_key
    CLOUDINARY_API_SECRET=your_cloudinary_api_secret
    ```
4.  **Start the Application:**
    Start both the backend server and frontend development server. 
    ```bash
    # Run backend (from backend directory)
    npm run dev
    
    # Run frontend (from frontend directory)
    npm run dev
    ```
