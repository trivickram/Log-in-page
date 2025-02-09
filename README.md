
---

# 🕷 **Spidy Login - Secure Authentication System**  

🚀 **Live Demo:** [Spidy Sigma](https://spidy-sigma.vercel.app/)  
🌐 **Backend API:** [Render Backend](https://log-in-page-tgu8.onrender.com/login)  
💼 **After Login Redirects To Portfolio:** [trivickram.vercel.app](https://trivickram.vercel.app/)  

---

## 📌 **Overview**  
Spidy Login is a **secure user authentication system** built using **Node.js, Express, MongoDB, and JWT** for authentication. The frontend is deployed on **Vercel**, and the backend is hosted on **Render**.  

✔ **User Features:**  
- **Register & Login securely** using **hashed passwords**.  
- **JWT-based authentication** to manage user sessions.  
- **Redirects to portfolio after login** with a **0.5s delay**.  
- **Error handling & validation** for smooth UX.  

✔ **Tech Stack:**  
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Node.js, Express, MongoDB (MongoDB Atlas)  
- **Authentication:** bcrypt.js + JWT  
- **Hosting:** Vercel (Frontend) & Render (Backend)  
- **Dockerized Backend** for easy deployment  

---

## 📁 **Project Structure**  
```plaintext
trivickram-log-in-page/
├── README.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── Back-End/
│   ├── index.js
│   ├── package-lock.json
│   ├── package.json
│   ├── .env
│   └── .gitignore
├── Front-End/
│   ├── LICENSE
│   ├── index.html
│   ├── register.html
│   ├── script.js
│   ├── styles.css
│   └── styles2.css
└── .github/
    └── ISSUE_TEMPLATE/
        ├── bug_report.md
        └── feature_request.md
```

---

## 🚀 **Setup & Installation**  

### **1️⃣ Clone the Repository**  
```sh
git clone https://github.com/trivickram/Log-in-page.git
cd Log-in-page
```

### **2️⃣ Install Backend Dependencies**  
```sh
cd Back-End
npm install
```

### **4️⃣ Start the Backend Server**  
```sh
node index.js
```
OR  
```sh
npm start
```

### **5️⃣ Run the Frontend**  
- Open `index.html` in a browser.  
- Modify `script.js` to connect it to your **backend API endpoint**.  

---

## 🔧 **API Endpoints**  

### **🔹 Register User**
```http
POST /register
```
**Request Body:**  
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "phone": "1234567890",
  "password": "securepassword"
}
```
**Response:**  
```json
{
  "message": "User registered successfully"
}
```

### **🔹 Login User**
```http
POST /login
```
**Request Body:**  
```json
{
  "email": "john@example.com",
  "password": "securepassword"
}
```
**Response:**  
```json
{
  "message": "Login successful",
  "token": "your-jwt-token"
}
```

---

## 🐳 **Docker Support**  

To run the backend in a **Docker container**, use the `Dockerfile` and `docker-compose.yml`.  

### **1️⃣ Build & Run Docker Container**  
```sh
docker-compose up --build
```

---

## 🛡 **Security Features**  
✅ **Password Hashing:** Uses `bcrypt.js` for securing passwords.  
✅ **JWT Authentication:** Secure session management.  
✅ **MongoDB Atlas (Cloud):** Database stored securely online.  
✅ **Environment Variables:** Secrets stored safely using `.env`.  

---

## 🤝 **Contributing**  
Want to contribute? Check out [CONTRIBUTING.md](CONTRIBUTING.md).  

---

## ⚖ **License**  
This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.  

---
