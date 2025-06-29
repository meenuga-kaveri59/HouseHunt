# 🏠 HouseHunt: Finding Your Perfect Rental Home

A MERN-based web application designed to simplify the process of finding and renting properties.  
HouseHunt connects renters with property owners through an intuitive platform that makes searching, booking, and managing rental properties easier, faster, and more secure.

---

## 📌 Project Overview
HouseHunt helps users:
- Find rental properties easily using advanced search filters
- View detailed listings with descriptions, photos, and prices
- Contact property owners/managers directly through the platform
- Complete rental transactions including booking and lease agreements securely within the app
- Property owners can manage their listings and bookings
- Admins oversee platform governance and user verification

---

## 🧩 Scenario-based Case Study
*Example: Renting an Apartment*

1️⃣ **User Registration:**  
Alice signs up as a renter, creating an account with her email and password.

2️⃣ **Browsing Properties:**  
After logging in, Alice sees a dashboard with available rental properties.  
She applies filters like location, rent range, and number of bedrooms to refine her search.

3️⃣ **Property Inquiry:**  
Alice finds a property she likes, views its details, and contacts the owner by filling out an inquiry form.

4️⃣ **Booking Confirmation:**  
The owner reviews and approves Alice's request. Alice gets a confirmation notification.

5️⃣ **Admin Approval:**  
Behind the scenes, the admin verifies and approves new property owners before they can list properties.

6️⃣ **Owner Management:**  
Bob, an owner, creates an account and adds/edits/deletes his properties once approved by the admin.

7️⃣ **Transaction & Lease Agreement:**  
Alice and Bob finalize the rental agreement and payment details through the app's messaging system.

8️⃣ **Move-in Process:**  
Alice successfully moves in, completing the process made possible by HouseHunt.

---

## 🛠 Technical Architecture

The app follows a client-server architecture:

| Layer     | Technology & Purpose                                                                        |
|---------|----------------------------------------------------------------------------------------------|
| Frontend | React.js + Axios + Bootstrap & Material UI → for responsive UI and REST API communication   |
| Backend  | Node.js + Express.js → handles business logic and API endpoints                             |
| Database | MongoDB → stores user data, properties, bookings, etc.                                       |
| Libraries| Moment.js, JWT, bcryptjs, multer, mongoose, dotenv                                           |

This architecture ensures:
- Real-time and secure data flow between frontend and backend
- Scalable and fast data storage
- Clear role-based flows for renters, owners, and admin users

---

## 📦 Folder Structure
/HouseHunt
/frontend ← React application
/backend ← Node.js & Express server

---
# ⚙️ HouseHunt – Setup & Deployment Guide

This guide explains how to:
- Install project dependencies
- Configure environment variables
- Run servers locally
- Deploy frontend & backend

---

## 📦 Step 1: Install Dependencies

After cloning/extracting the project, you’ll have:
- `/frontend` → React app
- `/backend` → Node.js & Express app

### 🟩 Frontend

cd frontend
npm install

### 🟦 Backend

cd ../backend
npm install

---

## 🔑 Step 2: Set Environment Variables

Keep sensitive info secure using `.env` files.

### 🟦 Backend → create `/backend/.env`:


MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
---

### 🟩 Frontend → create `/frontend/.env`:

REACT_APP_API_URL=http://localhost:5000

---

## ▶️ Step 3: Run Servers Locally

### 🟦 Start Backend

cd backend
npm start

Runs on: (http://localhost:5000)

---

### 🟩 Start Frontend

Open new terminal:

cd frontend
npm start

Runs on: (http://localhost:3000)

---

## ☁️ Step 4: Deployment

Deploy frontend & backend separately.

---

### 🟩 Frontend Deployment (Netlify / Vercel)

1. Build:

cd frontend
npm run build

2. Upload `build` folder to Netlify.

You’ll get:

```
https://your-frontend-site.netlify.app
```

---

### 🟦 Backend Deployment (Render / Railway)

1. Push project to GitHub.
2. Go to (https://render.com) → New Web Service.
3. Connect repo; set root as `/backend`.
4. Build command:

npm install

Start command:

npm start

5. Set env vars in Render:

* `MONGO_URI`
* `JWT_SECRET`

You’ll get:

```
https://your-backend-api.onrender.com
```

---

### 🔗 Connect Frontend to Backend in Production

Update `/frontend/.env`:

REACT_APP_API_URL=https://your-backend-api.onrender.com

Rebuild & redeploy frontend:

npm run build

Upload new build to Netlify.

---

✅ **Done!**
Your MERN app is now live! 🚀

```

✏️ Contributors
Meenuga Kaveri

✅ Conclusion
HouseHunt demonstrates how a MERN-based full-stack application can make renting properties easier and more secure, by combining user-friendly design with powerful backe

