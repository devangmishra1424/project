Studious - MERN scaffold (updated)

This project is a starter scaffold for the Studious app.
It contains a backend (Express + Mongoose) and a frontend (React + Vite).
Added features: Files Organizer & Important Links + Dashboard submit flow.

What’s included:
- backend/: Express server with auth (register/login), Goals API, Files and Links APIs.
- frontend/: React + Vite app with Login, Signup, Dashboard, Files, Links pages.
- JWT-based auth, frontend stores token in localStorage.

Requirements (locally):
- Node.js (v18+ recommended)
- MongoDB running locally (mongodb://localhost:27017). Alternatively, use MongoDB Atlas and set MONGO_URI in backend/.env

Quick start:
1) Backend
   cd backend
   npm install
   cp .env.example .env   # edit MONGO_URI & JWT_SECRET if needed
   npm run dev

2) Frontend
   cd frontend
   npm install
   npm run dev
   Open http://localhost:5173

Notes:
- File uploads are stored as base64 data URLs in MongoDB for convenience during development.
  Replace with S3/Supabase for production use.
- Dashboard "Submit" button opens the attached file and the submission link in new tabs.
