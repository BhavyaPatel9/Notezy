# 📝 Notezy - Simple Note-Taking App (MERN Stack) | **[🔗 Live Demo (Render)](https://notezy-2fs4.onrender.com/)**

Notezy is a Full-Stack Note-Taking Web Application built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js).  
It allows users to **Create, Read, Update, and Delete notes** (CRUD functionality) with title and description.  
This project demonstrates a fully functional **REST API**, a responsive React frontend, and modern backend features like **rate limiting using Upstash Redis**.

---

## 🚀 Features

- ✨ **Create, Update, and Delete Notes** with Title & Description
- 🛠️ **Fully Functional REST API** built and tested with tools like Postman
- ⚙️ **Rate Limiting** (using Upstash Redis) — practical implementation of a real-world backend concept
- 📱 **Completely Responsive Frontend UI** (works on mobile, tablet, and desktop)
- 🌐 Covers **HTTP Methods, Status Codes, SQL vs NoSQL** concepts
- ☁️ Ready for production deployment on platforms like Vercel, Render, and Railway

---

## 🏗️ Tech Stack

| Frontend | Backend | Database | Other |
|----------|---------|----------|-------|
| React.js | Node.js + Express.js | MongoDB Atlas | Axios, CORS, Dotenv, Upstash Redis, Rate Limiter |

---

## 🗃️ API Endpoints (RESTful)

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/notes` | Get all notes |
| GET | `/api/notes/:id` | Get a single note |
| POST | `/api/notes` | Create a new note |
| PUT | `/api/notes/:id` | Update an existing note |
| DELETE | `/api/notes/:id` | Delete a note |

---

-----

# 🚀 Notezy: Local Development & Deployment Guide

This guide will walk you through setting up and running the Notezy application locally, along with essential `.env` configurations.

-----

## 1\. **Clone the Repository**

To get started, clone the Notezy repository to your local machine and navigate into the project directory:

```bash
git clone https://github.com/BhavyaPatel9/Notezy.git
cd Notezy
```

-----

## 2\. **Environment Variables Setup (.env)**

Both the backend and frontend require specific environment variables to function correctly.

### 2.1. Backend (`/backend`)

Create a file named `.env` in the `backend/` directory. Populate it with your specific credentials:

```
MONGO_URI=<your_mongo_uri>
UPSTASH_REDIS_REST_URL=<your_redis_rest_url>
UPSTASH_REDIS_REST_TOKEN=<your_redis_rest_token>
NODE_ENV=development # Set to 'production' for deployment environments
```

  * `MONGO_URI`: Your MongoDB connection string.
  * `UPSTASH_REDIS_REST_URL`: Your Upstash Redis REST URL.
  * `UPSTASH_REDIS_REST_TOKEN`: Your Upstash Redis REST token.
  * `NODE_ENV`: Specifies the environment; use `development` for local setup and `production` for deployed instances.

-----

## 3\. **Run the Application**

### 3.1. Run the Backend

Navigate into the `backend/` directory, install the necessary dependencies, and then start the development server:

```bash
cd backend
npm install
npm run dev
```



### 3.2. Run the Frontend

In a **separate terminal window**, navigate to the `frontend/` directory, install its dependencies, and launch the development server:

```bash
cd frontend
npm install
npm run dev
```



-----
