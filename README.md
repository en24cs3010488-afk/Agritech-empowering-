# AgriTech – Empowering Farmers (MERN Starter)

A beginner-friendly full-stack starter project aligned with the SmartBridge project brief.

## Stack
- Frontend: React + Vite + Bootstrap
- Backend: Node.js + Express
- Database: MongoDB (Mongoose)
- Authentication: JWT + bcryptjs
- Roles: farmer / admin

## Requirements
Install Node.js LTS (Node 18+ recommended) and MongoDB locally, or create a MongoDB Atlas database.

## Setup

### 1) Backend
Open a terminal in `backend`:
```bash
npm install
```
Copy `.env.example` to `.env`, then set `MONGO_URI` and `JWT_SECRET`.
```bash
npm run dev
```
Backend runs at http://localhost:5000

### 2) Frontend
Open another terminal in `frontend`:
```bash
npm install
npm run dev
```
Open the URL Vite prints (usually http://localhost:5173).

## Demo flow
1. Register a farmer account.
2. Login.
3. Add farm/crop information from the dashboard.
4. Explore weather/pest alert demo cards.
5. Admin endpoints are role-protected; to make an admin, manually change a user's `role` to `admin` in MongoDB after registration.

## Important
- Weather and market prices are clearly marked as demo/sample data. Connect a real weather/market API before claiming live data.
- This is a learning starter, not a production-hardened system. Before public deployment, add rate limiting, email verification, password reset, stronger validation, audit logs, and secure deployment settings.
