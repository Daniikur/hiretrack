# HIRETRACK AI

HireTrack AI is a modern AI-powered job application tracking platform built with React, FastAPI, MongoDB Atlas, and Groq AI.

The platform helps users manage job applications, resumes, interview notes, analytics, and AI-powered job description summaries in one place.

---

# Features

- AI Job Description Summarization
- Resume Management
- Application Tracking Pipeline
- Analytics Dashboard
- Interview Notes
- Authentication System
- MongoDB Atlas Database
- Groq AI Integration
- FastAPI Backend
- React Frontend
- Responsive Modern UI

---

# Tech Stack

## Frontend

- React.js
- Tailwind CSS
- CRACO
- Axios
- React Router

## Backend

- FastAPI
- Python
- MongoDB Atlas
- Motor
- JWT Authentication
- Groq AI API

---

# Project Structure

```bash
hiretrack/
│
├── frontend/
├── backend/
├── uploads/
├── README.md
```

---

# Installation

## 1. Clone Project

```bash
git clone <your_repository_url>
cd hiretrack
```

---

# Backend Setup

## 1. Create Virtual Environment

```bash
cd backend
python -m venv venv
```

## 2. Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### Mac/Linux

```bash
source venv/bin/activate
```

---

## 3. Install Backend Packages

```bash
pip install -r requirements.txt
```

---

## 4. Configure Environment Variables

Create a `.env` file inside the `backend` folder:

```env
MONGO_URL=your_mongodb_connection
DB_NAME=hiretrack
JWT_SECRET=your_secret_key
GROQ_API_KEY=your_groq_api_key
```

---

## 5. Run Backend

```bash
uvicorn server:app --reload
```

Backend runs on:

```bash
http://127.0.0.1:8000
```

---

# Frontend Setup

Open a new terminal:

```bash
cd frontend
```

---

## Install Frontend Packages

```bash
npm install --legacy-peer-deps
```

---

## Start Frontend

```bash
npm start
```

Frontend runs on:

```bash
http://localhost:3000
```

---

# MongoDB Atlas Setup

1. Create MongoDB Atlas account
2. Create a cluster
3. Add a database user
4. Add your IP address
5. Copy the connection string
6. Paste it into backend `.env`

Example:

```env
MONGO_URL=mongodb+srv://username:password@cluster.mongodb.net/
```

---

# AI Integration

This project uses Groq AI for:

- Resume analysis
- Job description summarization
- AI insights

Supported model:

```bash
llama-3.3-70b-versatile
```

---

# Build Frontend

```bash
npm run build
```

Production build will be generated in:

```bash
frontend/build
```

---

# API Endpoints

## Authentication

```http
POST /api/auth/register
POST /api/auth/login
```

---

## Applications

```http
GET    /api/applications
POST   /api/applications
PUT    /api/applications/{id}
DELETE /api/applications/{id}
```

---

## AI Features

```http
POST /api/ai/summarize
POST /api/applications/{id}/summarize
```

---

# Environment Variables

## Backend `.env`

```env
MONGO_URL=
DB_NAME=
JWT_SECRET=
GROQ_API_KEY=
```

---

## Frontend `.env`

```env
REACT_APP_BACKEND_URL=http://127.0.0.1:8000
```

---

# Screenshots

- Dashboard
- Job Applications
- AI Summarizer
- Analytics
- Resume Manager

---

# Author

## Kurmanzhan Daniiarbek Kyzy

GitHub:  
https://github.com/Daniikur

---

# License

This project is for educational and portfolio purposes.