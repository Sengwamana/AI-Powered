# AI-Powered Chat App

An AI-powered full-stack web application featuring secure user authentication, intelligent conversations using Google's Generative AI, image handling via ImageKit, and a sleek React frontend. Developed by Sengwamana Emeran.

---

## 📑 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Usage](#usage)
- [Configuration](#configuration)
- [Examples](#examples)
- [Troubleshooting](#troubleshooting)
- [Contributors](#contributors)
- [License](#license)

---

## 🧠 Introduction

This project combines modern AI technologies with a clean frontend experience, enabling users to engage in dynamic conversations powered by Google's Generative AI. The app is designed to support image uploads and intelligent interactions, with user management handled by Clerk authentication.

---

## ✨ Features

- 🔐 Secure authentication with Clerk
- 🤖 AI-generated chat responses using `@google/generative-ai`
- 🖼️ Image upload & CDN optimization via ImageKit
- ⚛️ React frontend with smooth animations and routing
- 🔄 State & server caching via React Query
- 🧵 Markdown support in chat responses

---

## 🛠️ Tech Stack

### Frontend

- React 18
- Vite
- Clerk for Auth (`@clerk/clerk-react`)
- React Router DOM
- React Markdown
- React Type Animation
- React Query
- ESLint

### Backend

- Node.js with Express
- MongoDB (via Mongoose)
- Clerk SDK for server-side auth
- ImageKit SDK
- CORS

---

## 🚀 Installation

### 📦 Backend Setup

```bash
# Navigate to backend folder
cd backend

# Install dependencies
npm install

# Start the backend (with environment variables)
npm start

# Navigate to frontend folder (e.g., aichatstarter)
cd aichatstarter

# Install dependencies
npm install

# Run the development server
npm run dev

⚙️ Configuration
Required .env for Backend
Create a .env file in the backend directory with:

PORT=5000
MONGODB_URI=your_mongo_db_connection_string
CLERK_SECRET_KEY=your_clerk_secret
IMAGEKIT_PUBLIC_KEY=your_public_key
IMAGEKIT_PRIVATE_KEY=your_private_key
IMAGEKIT_URL_ENDPOINT=https://ik.imagekit.io/your_endpoint/

💡 Usage
Once both servers are running:

Open the frontend in your browser (usually at http://localhost:5173).

Sign in via Clerk.

Start chatting with the AI!

Upload and send images seamlessly.

📌 Examples
Chat: Users type queries, and the backend uses Google's Generative AI to respond.

Image Upload: Images are uploaded through ImageKit and displayed in the UI.

Markdown: Chat supports markdown formatting like **bold**, *italic*, etc.

🛠️ Troubleshooting
Make sure MongoDB is running and the URI is correct.

Verify your Clerk and ImageKit keys are valid and properly scoped.

CORS issues? Ensure frontend and backend ports are allowed in CORS middleware.

👥 Contributors
Sengwamana Emeran – Developer & Maintainer

📄 License
This project is licensed under the ISC License.
