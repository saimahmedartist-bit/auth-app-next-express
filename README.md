# 🔐 Secure Auth System – Next.js + Express + MongoDB

This project is the **Day 1 foundation** of a full-stack modern authentication system. It includes:

- A frontend built with **Next.js**
- A backend built with **Node.js + Express**
- Secure user authentication using **bcryptjs** for password hashing
- **MongoDB** database integration using **Mongoose**
- Modular structure and environment configuration

---

## 📁 Project Structure

task-1/
├── backend/
│ ├── controllers/
│ ├── models/
│ ├── routes/
│ ├── middleware/
│ ├── server.js
│ └── .env
└── frontend/
├── pages/
│ ├── login.js
│ └── register.js
└── components/

yaml
Copy
Edit

---

## 🔧 Core Features Implemented (Day 1)

### ✅ Backend (Express.js)
- POST `/api/register`: Register new user with hashed password
- POST `/api/login`: Login by verifying email + hashed password
- MongoDB connected via Mongoose
- Passwords hashed using `bcryptjs` with 10 salt rounds
- Environment variables securely managed in `.env`

### ✅ Frontend (Next.js)
- `/register`: Form to register with name, email, password
- `/login`: Form to login with email, password
- Axios used to connect frontend to backend
- Simple form validation (no empty inputs)
- Error and success message display

---

## ⚙️ Technologies Used

### 🖥️ Frontend
- Next.js
- React
- Axios

### 🌐 Backend
- Node.js
- Express.js
- Mongoose (MongoDB)
- bcryptjs
- dotenv
- cors

---

## 🛡️ Security & Best Practices

- ✅ Passwords never stored in plain text (bcrypt hash used)
- ✅ All environment secrets stored in `.env`
- ✅ Email uniqueness validated on backend
- ✅ Modular route-controller-model structure
- ✅ Clear separation between frontend and backend
- ✅ Error handling implemented in both frontend & backend

---

## 📦 Getting Started

### Clone the repository
```bash
git clone https://github.com/your-username/secure-auth-jwt-nextjs-express.git
cd secure-auth-jwt-nextjs-express
Setup Backend
bash
Copy
Edit
cd backend
npm install
touch .env
# Add your environment variables to the .env file
# Example:
# MONGO_URI=mongodb+srv://...
# PORT=5000

npm run dev
Setup Frontend
bash
Copy
Edit
cd frontend
npm install
npm run dev
🌍 API Routes
Method	Route	Description
POST	/api/register	Register new user
POST	/api/login	Login and return JWT

📂 Environment Variables
Create a .env file in the backend directory:

ini
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

👤 Author
Saim Ahmed – @saimahmedartist-bit

