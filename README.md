# 💬Vibe: A Full-Featured Real-Time Messaging Application
This is a comprehensive, real-time chat application built using the **MERN Stack** (MongoDB, Express.js, React, Node.js). It integrates **Firebase** for reliable file storage and leverages **Socket.IO** for instant, bi-directional communication, enabling a seamless messaging experience.
 
## ⚠️ **Important Security Warning:**
Messages sent in direct messages and group chats are **not encrypted** and are stored as **plain text in the database.**
DO NOT share sensitive information, such as passwords, financial details, or any private data that you use in other applications or accounts. Use this application strictly for demonstration or non-sensitive communication purposes.
 
## 🚩 Live Demo
Current version running at:
### Note:
It may take up to 1 minute for the site to be brought up while the loading indicator is displayed. This delay occurs because free hosting instances may spin down with inactivity.

## ✨ Features
* **Authentication & Profile:** Supports user signup, sign-in, initial profile setup, and profile updates.
* **Friend Management:** Add new contacts by sending, approving, or rejecting friend requests.
* **Group Messaging:** Create and manage group chats.
* **Real-Time Chatting:** Instant, real-time communication in both direct messages and group environments.
* **Media Support:** Send images and various other files within chat conversations.
* **Search & Filtering:**
    * Filter your chats to display all, DMs, or groups.
    * Search for specific chats or friend requests.
* **Information View:**
    * View a friend's profile to see contact information, groups in common, and shared files.
    * View group details, including creation date, members, and shared files.
 
## ⚙ Setup
### 1. Server Configuration
Create a **.env** file in the `server` folder with the following variables:
```bash
PORT=3001
JWT_KEY="YOUR_JWT_KEY"
ORIGIN="http://localhost:3000"
DATABASE_URL="YOUR_DATABASE_URL"
PEPPER_STRING="YOUR_PEPPER_STRING"
```

### 2. Client Configuration
Create a **.env** file in the `client` folder with your Firebase and server connection details:
```bash
VITE_FIREBASE_API_KEY="YOUR_API_KEY"
VITE_FIREBASE_AUTH_DOMAIN="YOUR_AUTH_DOMAIN"
VITE_FIREBASE_PROJECT_ID="YOUR_PROJECT_ID"
VITE_FIREBASE_STORAGE_BUCKET="YOUR_STORAGE_BUCKET"
VITE_FIREBASE_MESSAGING_SENDER_ID="YOUR_MESSAGING_SENDER_ID"
VITE_FIREBASE_APP_ID="YOUR_APP_ID"
VITE_SERVER_URL="http://localhost:3001"
```

## 🏃‍♂️ Running in Local Development Mode
### Server (Backend)
Navigate to the server directory:
```bash
cd server
npm install 
npm run dev
```
### Client (Frontend)
Navigate to the client directory:
```bash
cd client
npm install
npm run dev
```

Open http://localhost:3000 with your browser to see the result.
