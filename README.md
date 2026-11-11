# CiviGuard-AI

A civic issue reporting platform: citizens submit complaints, and admins track and manage them, with maps in the UI and AI assistance on the backend.

## What it includes

- **Authentication** - email/password with JWT, plus Google sign-in (Passport)
- **Complaints** - complaint submission and management, with separate admin routes
- **Maps** - Mapbox GL and react-leaflet maps in the frontend
- **AI** - Google Gemini integration on the backend
- **Seed data** - a script to load initial data

## Tech stack

- **Frontend:** React 18 + TypeScript, Vite, Tailwind CSS, react-router, Mapbox GL, react-leaflet
- **Backend:** Node.js, Express, TypeScript, MongoDB (Mongoose), JWT, Passport (Google OAuth + JWT strategies), @google/generative-ai

## Project structure

```
frontend/   React app (Vite)
backend/    Express API
  src/routes/        auth, complaints, admin
  src/controllers/   complaint controllers
  src/scripts/       seed script
```

## Getting started

Backend:

```bash
cd backend
npm install
# configure environment variables for the database, auth and API keys
npm run dev
npm run seed   # optional: load seed data
```

Frontend:

```bash
cd frontend
npm install
npm run dev
```
