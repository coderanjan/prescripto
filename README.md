# 🏥 Prescripto

Prescripto is a full-stack doctor appointment booking platform built with the MERN stack. Patients can discover doctors, book appointments, make online payments, and manage their profiles, while doctors and admins can manage appointments and platform data.

## 🔗 Live Demo

| Application         | Link                                                           |
| ------------------- | -------------------------------------------------------------- |
| 🌐 Patient Frontend | [Prescripto](https://prescripto-frontend-kok2.onrender.com/)   |
| 🛠️ Admin Panel     | [Admin Dashboard](https://prescripto-admin-tkj9.onrender.com/) |
| 💻 Source Code      | [GitHub Repository](https://github.com/coderanjan/prescripto)  |

> ⚠️ The application is deployed on Render's free tier. After a period of inactivity, the first request may take some time while the service starts.

## ✨ Features

### 👤 Patient

* Register and log in
* Browse doctors by specialty
* View doctor profiles and availability
* Book appointments
* Cancel appointments
* Make online payments
* View appointment history
* Update profile information
* Upload profile images

### 🩺 Doctor

* Secure doctor authentication
* View appointments
* Manage appointment status
* View earnings and dashboard statistics
* Update doctor profile
* Manage availability

### 🛠️ Admin

* Secure admin authentication
* Add and manage doctors
* View registered doctors
* View and manage appointments
* View platform statistics
* Manage doctor availability

### 🔐 Security & Backend

* JWT-based authentication
* Role-based access control
* Password hashing
* Protected API routes
* MongoDB data persistence
* Cloudinary image storage
* Razorpay payment integration

## 🧰 Tech Stack

### Frontend

* React
* Vite
* React Router
* Tailwind CSS
* Axios
* Context API
* React Toastify

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcrypt
* Multer
* Cloudinary
* Razorpay

### Deployment

* Render

## 🏗️ Project Structure

```text
prescripto/
│
├── frontend/          # Patient-facing React application
│
├── admin/             # Admin/doctor dashboard
│
└── backend/           # Express.js REST API
    ├── config/
    ├── controllers/
    ├── middleware/
    ├── models/
    ├── routes/
    └── server.js
```

## 🔄 Application Flow

```text
Patient
   │
   ▼
React Frontend
   │
   ▼
Express REST API
   │
   ├── Authentication / Authorization
   ├── Appointment Management
   ├── Payment Processing
   └── Image Upload
   │
   ├── MongoDB
   ├── Cloudinary
   └── Razorpay
```

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

* Node.js 18+
* npm
* MongoDB / MongoDB Atlas account
* Cloudinary account
* Razorpay account

### 1. Clone the repository

```bash
git clone https://github.com/coderanjan/prescripto.git

cd prescripto
```

### 2. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` directory:

```env
PORT=4000
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key

RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret

ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
```

Start the backend:

```bash
npm run server
```

### 3. Frontend Setup

Open a new terminal:

```bash
cd frontend
npm install
```

Create a `.env` file:

```env
VITE_BACKEND_URL=http://localhost:4000
```

Start the frontend:

```bash
npm run dev
```

The frontend will normally run at:

```text
http://localhost:5173
```

### 4. Admin Panel Setup

```bash
cd admin
npm install
```

Create the required environment file:

```env
VITE_BACKEND_URL=http://localhost:4000
```

Start the admin application:

```bash
npm run dev
```

## 💳 Payment

Prescripto uses Razorpay for online appointment payments.

For development, use Razorpay test mode and test credentials. Never commit production API keys or secrets to GitHub.

## 🖼️ Image Upload

User and doctor profile images are uploaded through the backend using Multer and stored on Cloudinary.

```text
Client
  ↓
Multer
  ↓
Backend
  ↓
Cloudinary
  ↓
Image URL
  ↓
MongoDB
```

MongoDB stores the image URL rather than the actual image file.

## 📸 Screenshots

### Patient Application

*Add screenshots here.*

### Doctor Dashboard

*Add screenshots here.*

### Admin Dashboard

*Add screenshots here.*

## 🌐 Deployment

The application is deployed using Render.

The frontend, admin panel, and backend are deployed as separate services.

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature/your-feature
```

3. Commit your changes

```bash
git commit -m "Add some feature"
```

4. Push the branch

```bash
git push origin feature/your-feature
```

5. Open a Pull Request

## 📄 License

This project is available under the [MIT License](https://github.com/coderanjan/prescripto/blob/main/LICENSE).

## 📬 Contact

Maintained by [@coderanjan](https://github.com/coderanjan).

For questions, bug reports, or suggestions, please open an issue in the repository.
