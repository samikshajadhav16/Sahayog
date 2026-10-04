# 🚀 Sahayog — Bridge of Service

Sahayog is a **field workforce management system** designed for civic sanitation operations. It helps non-governmental organizations efficiently manage field workers involved in **waste collection, recycling drives, and public awareness campaigns many more**.

---

## 🚀 Why Sahayog?

Municipal systems often rely on **manual processes (paper/phone calls)** which lead to:
- ❌ Ghost attendance  
- ❌ Lack of accountability  
- ❌ No real-time tracking  
- ❌ Poor data insights  

Sahayog solves this by providing a **digital, transparent, and accountable system** for managing field operations.

---

## 🏗️ System Architecture (Three-Tier)

### 1️⃣ Frontend (React)
- ⚛️ React + Vite
- 🎨 Tailwind CSS
- 🌐 Runs on `http://localhost:5173`
- 🔗 Communicates with backend via Axios

### 2️⃣ Backend (Node.js + Express)
- 🟢 Node.js + Express
- 🔐 Handles authentication & business logic
- 📡 REST API at `/api/...`
- 🗄️ MongoDB (via Mongoose)
- 🌐 Runs on `http://localhost:5000`

### 3️⃣ AI Microservice (Python + Flask)
- 🧠 Face Recognition using `face_recognition` (dlib)
- 🔗 Communicates with Node via HTTP
- 🌐 Runs on `http://localhost:5001`

---

## 🗄️ Database & Cloud Storage

- ☁️ MongoDB Atlas (Cloud Database)
- 📁 Database Name: `sevasetu`
- 🔄 Shared access:
  - Node.js → Mongoose
  - Python → PyMongo  

- 🖼️ **Cloudinary** used for:
  - Image storage (face data, uploads)
  - Secure cloud-based media management
  - Fast retrieval for verification

---

## 👥 User Roles

### 👑 ADMIN
- Full system access
- 📊 Analytics dashboard
- 👤 User management
- 📅 Leave calendar
- 🚨 Alerts monitoring

---

### 🧑‍💼 TEAM_LEAD
- 📌 Creates & assigns tasks
- ✅ Reviews attendance
- 📝 Approves/rejects leaves
- 📄 Submits field reports

---

### 👷 FIELD_WORKER
- 📍 Check-in/out (Face + GPS)
- 📝 Submit reports
- 🌴 Request leave
- 📋 View assigned tasks

---

## ✨ Key Features

- 📍 **Geo-tagged Attendance**
- 🧠 **Face Recognition Verification**
- 🖼️ **Cloud Image Storage (Cloudinary)**
- 📊 **Role-based Dashboards**
- 📄 **Digital Field Reporting**
- 🌴 **Leave Management System**
- 📈 **Analytics & Insights**

---

## 🛠️ Tech Stack

| Layer        | Technology |
|-------------|-----------|
| Frontend    | React, Vite, Tailwind CSS |
| Backend     | Node.js, Express |
| Database    | MongoDB Atlas |
| AI Service  | Python, Flask, face_recognition |
| Cloud       | Cloudinary |
| Communication | REST APIs |

---

## ⚙️ Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/your-username/seva-setu.git
cd seva-setu
```

### 2. Setup Backend
```bash
cd server
npm install
npm run dev
```

### 3. Setup Frontend
```bash
cd client
npm install
npm run dev
```

### 4. Setup Python Service
```bash
cd python_service
pip install -r requirements.txt
python app.py
```

---

## 🔐 Environment Variables

Create `.env` files in respective folders:

### Backend (`server/.env`)
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PYTHON_SERVICE_URL=http://localhost:5001
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

---

## 📌 Future Enhancements

- 📱 Mobile app for field workers
- 🔔 Real-time notifications
- 📊 Advanced analytics dashboard
- 🌐 Multi-city scalability

---

## 🌟 Tagline

> _"Bridging the gap between service and accountability."


##  Architecture Diagram

<img width="1390" height="1600" alt="image" src="https://github.com/user-attachments/assets/628fd117-bab9-4c66-8309-bdb7e74d7dae" />



## System Overview
<img width="1899" height="880" alt="image" src="https://github.com/user-attachments/assets/bc3ea59f-db2f-4c25-804b-db788afa29f5" />
<img width="1913" height="892" alt="image" src="https://github.com/user-attachments/assets/32d691b6-eb50-4771-9b81-cbc8c1e749ee" />

## worker Dashboard
<img width="956" height="436" alt="image" src="https://github.com/user-attachments/assets/58c92705-f6ff-4954-bd90-18dadbd4cb22" />
<img width="957" height="439" alt="image" src="https://github.com/user-attachments/assets/17c742ca-a89b-4462-badb-e5071c53322c" />
<img width="953" height="431" alt="image" src="https://github.com/user-attachments/assets/09ac6c29-d06e-43b8-adac-fed2ec49d908" />
<img width="956" height="435" alt="image" src="https://github.com/user-attachments/assets/351ced3f-c141-42a4-adbc-1af15d211172" />
<img width="959" height="426" alt="image" src="https://github.com/user-attachments/assets/26610c01-bc53-4ab2-bab9-182eef57e5ef" />

--------------------------------------------------------------------------------------------------------------------------

## Team Lead Dashboard 
<img width="956" height="427" alt="image" src="https://github.com/user-attachments/assets/6bb48f22-9ee2-4f62-8dd7-f40b3ed25c14" />
<img width="954" height="435" alt="image" src="https://github.com/user-attachments/assets/8411ed34-e71c-4b4a-94b2-d2d9676e879a" />
<img width="959" height="423" alt="image" src="https://github.com/user-attachments/assets/f412883b-f151-4b24-9db7-684b89b2ff9e" />

-----------------------------------------------------------------------------------------------------------------------------

## Admin Dashboard
<img width="951" height="439" alt="image" src="https://github.com/user-attachments/assets/0d1214ca-d0a4-4743-9f6e-bbe9f44c6e69" />
<img width="959" height="439" alt="image" src="https://github.com/user-attachments/assets/ddab049b-9c7f-4498-aa95-d683a53694ff" />








