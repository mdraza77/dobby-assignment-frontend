# 🚀 Dobby Drive - Frontend (React + Vite)

Dobby Drive is a full-stack cloud storage application built with the **MERN** stack. It allows users to manage folder structures, upload images with specific metadata, and track storage usage in real-time.

## 📁 Local Project Structure

To manage the project efficiently, keep both repositories inside a single parent directory.

```text
dobby_drive/
├── backend/  (Node.js/Express API)
└── frontend/ (React App - This Repository)
```

---

## ⚙️ Installation & Local Setup

Follow these steps to set up the environment on your machine:

### 1. Main Directory & Cloning

Create a root folder and clone both repositories:

```bash
# Create main folder
mkdir dobby_drive
cd dobby_drive

# Clone Backend repository
git clone https://github.com/mdraza77/dobby-assignment-backend.git

# Clone Frontend repository
git clone https://github.com/mdraza77/dobby-assignment-frontend.git
```

### 2. Backend Configuration

Navigate to the backend folder and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file in the backend root and add your credentials:

```env
MONGO_URI=mongodb+srv://dobby_db:ATqqlCFLbIfxFIcW@cluster0.fl1u6n2.mongodb.net/?appName=Cluster0
JWT_SECRET=raza_secret_key_123
```

Start the API:

```bash
npm start
```

### 3. Frontend Configuration (This Repo)

Open a new terminal, navigate to the frontend folder, and install dependencies:

```bash
cd dobby-assignment-frontend
npm install
```

#### API Configuration

Ensure `src/api.js` points to your production backend URL:

```js
const API = axios.create({ baseURL: "https://dobby-assignment-backend.onrender.com/api" });
```

Start the app:

```bash
npm run dev
```

---

## ✨ Features & Requirements

### 🎨 Design & Logic

The application features a modern UI built with Tailwind CSS and Lucide React icons. It is designed to meet specific technical requirements:

- **Recursive Folder Size (Requirement #5):** Every folder dynamically calculates and displays its total size, including all images within nested sub-folders at any depth.
- **Mandatory Image Metadata (Requirement #6):** The upload interface requires both a Name and an Image File. Uploads are blocked unless both fields are provided.
- **Cloud Database:** Utilizes MongoDB Atlas for persistent storage of users, folders, and file metadata.
- **Responsive Dashboard:** A clean, professional interface for navigating the cloud drive using breadcrumbs.

### 🌐 Deployment

- **Frontend:** Hosted on Netlify
- **Backend:** Hosted on Render
- **Database:** MongoDB Atlas (Global Cluster)

---

## 👤 Test Credentials

Use the following credentials for testing:

- **Email:** mdraza8397@gmail.com
- **Password:** Success2026$

---

## 📌 Notes

- This repository contains only the frontend React/Vite application.
- The backend API lives in the `dobby-assignment-backend` repository.
- Make sure the backend is running before starting the frontend app.

---

## 📄 Backend Reference

The source code for the backend API can be found in the Dobby Backend Repository.
