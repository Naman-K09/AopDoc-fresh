# 🏥 AopDoc - Doctor Appointment System

> A modern, full-stack web application for seamless doctor appointment management and scheduling.

[![GitHub Stars](https://img.shields.io/github/stars/Naman-K09/AopDoc?style=social)](https://github.com/Naman-K09/AopDoc)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/node.js-v14+-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18.0+-61dafb.svg)](https://reactjs.org/)

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🏗️ Project Structure](#-project-structure)
- [🛠️ Tech Stack](#-tech-stack)
- [🚀 Quick Start](#-quick-start)
- [📡 API Routes](#-api-routes)
- [💡 How to Use](#-how-to-use)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 👥 **User Management** | Register and manage patient profiles securely |
| 🩺 **Doctor Management** | Add, update, and manage doctor information and availability |
| 📅 **Smart Booking** | Intuitive appointment scheduling with real-time availability |
| 📊 **Admin Dashboard** | Comprehensive admin panel for oversight and management |
| 🔐 **Authentication** | Secure JWT-based authentication and authorization |
| 📱 **Responsive UI** | Mobile-friendly React frontend |
| ⚡ **Fast API** | Express.js backend with optimized performance |
| 💾 **Data Persistence** | MongoDB for reliable data storage |

---

## 🏗️ Project Structure

```
AopDoc/
├── 📂 client/                          # React Frontend
│   ├── build/                         # Production build
│   ├── src/                          # Source code
│   └── package.json
├── 📂 config/
│   └── db.js                         # 🔌 Database configuration
├── 📂 controllers/
│   ├── userCtrl.js                   # User logic
│   ├── doctorCtrl.js                 # Doctor logic
│   └── adminCtrl.js                  # Admin logic
├── 📂 middlewares/
│   └── authMiddleware.js             # 🔐 Auth middleware
├── 📂 models/
│   ├── userModels.js                 # User schema
│   ├── doctorModel.js                # Doctor schema
│   └── appointmentModel.js           # Appointment schema
├── 📂 routes/
│   ├── userRoutes.js                 # User endpoints
│   ├── doctorRoutes.js               # Doctor endpoints
│   └── adminRoutes.js                # Admin endpoints
├── server.js                         # 🚀 Express server
└── package.json                      # Dependencies
```

---

## 🛠️ Tech Stack

### Frontend
- ⚛️ **React.js** - UI library
- 🎨 **CSS/Bootstrap** - Styling
- 📡 **Axios** - HTTP client

### Backend
- 🟢 **Node.js** - Runtime
- ⚡ **Express.js** - Web framework
- 🔐 **JWT** - Authentication
- 💾 **MongoDB** - NoSQL database

### Tools & Services
- 📦 **npm** - Package manager
- 🔧 **Git** - Version control

---

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- MongoDB installed or MongoDB Atlas account
- Git

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Naman-K09/AopDoc.git
   cd AopDoc
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   - Edit `config/db.js` with your MongoDB connection string
   - Set up environment variables if needed

4. **Start the server**
   ```bash
   npm start
   ```

5. **Access the application**
   - Open your browser and navigate to `http://localhost:5000`
   - 🎉 You're ready to go!

---

## 📡 API Routes

### 👤 User Routes
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/user/register` | Register new user |
| `POST` | `/api/user/login` | User login |
| `GET` | `/api/user/profile` | Get user profile |
| `PUT` | `/api/user/profile` | Update user profile |
| `GET` | `/api/user/appointments` | Get user appointments |

### 🩺 Doctor Routes
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/doctor/list` | Get all doctors |
| `POST` | `/api/doctor/create` | Add new doctor (Admin) |
| `GET` | `/api/doctor/:id` | Get doctor details |
| `PUT` | `/api/doctor/:id` | Update doctor info |
| `GET` | `/api/doctor/:id/availability` | Check availability |

### ⚙️ Admin Routes
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/admin/users` | List all users |
| `GET` | `/api/admin/doctors` | List all doctors |
| `GET` | `/api/admin/appointments` | View all appointments |
| `DELETE` | `/api/admin/user/:id` | Remove user |
| `DELETE` | `/api/admin/doctor/:id` | Remove doctor |

### 📅 Appointment Routes
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/appointment/book` | Book appointment |
| `GET` | `/api/appointment/:id` | Get appointment details |
| `PUT` | `/api/appointment/:id` | Reschedule appointment |
| `DELETE` | `/api/appointment/:id` | Cancel appointment |

---

## 💡 How to Use

### For Patients 👥

1. **Create Account**
   - Click "Register" on the homepage
   - Enter your details and create a password

2. **Browse Doctors**
   - Go to "Find Doctors" section
   - Filter by specialty, location, or availability

3. **Book Appointment**
   - Select your preferred doctor
   - Choose available time slot
   - Confirm and receive confirmation

4. **Manage Appointments**
   - View all your appointments in the dashboard
   - Reschedule or cancel if needed

### For Doctors 🩺

1. **Create Profile**
   - Register as a doctor
   - Add specialization and qualifications

2. **Manage Schedule**
   - Set your availability
   - View appointment bookings

3. **Update Information**
   - Update consultation fees
   - Modify contact information

### For Administrators ⚙️

1. **Access Dashboard**
   - Login with admin credentials
   - Monitor all users, doctors, and appointments

2. **Manage Users**
   - View, edit, or remove user accounts
   - Handle user-related issues

3. **Monitor System**
   - Track appointment analytics
   - Generate reports

---

## 🔒 Security Features

- ✅ **JWT Authentication** - Secure token-based auth
- ✅ **Password Hashing** - Bcrypt encryption
- ✅ **Role-Based Access** - Separate permissions for users/doctors/admins
- ✅ **Protected Routes** - Middleware validation
- ✅ **Input Validation** - Server-side validation

---

## 👨‍💻 Author

**Naman K**
- GitHub: [@Naman-K09](https://github.com/Naman-K09]

</div>
