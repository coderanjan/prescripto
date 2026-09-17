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

<img width="957" height="470" alt="image" src="https://github.com/user-attachments/assets/fbafc94e-1ba0-4822-b56b-03d2e34e7ee1" />
<img width="955" height="468" alt="image" src="https://github.com/user-attachments/assets/765fdd20-011a-4dfb-b9b5-6d09213dde04" />
<img width="937" height="305" alt="image" src="https://github.com/user-attachments/assets/ece4d56c-294d-4a87-b7dc-5c5f02c519f6" />



### Doctor Dashboard

<img width="956" height="461" alt="image" src="https://github.com/user-attachments/assets/61e3553e-1c41-471e-a68b-50e881305ab6" />
<img width="955" height="464" alt="image" src="https://github.com/user-attachments/assets/05c7c703-89fc-4cc7-b5b0-6596a3d15fcd" />
<img width="944" height="461" alt="image" src="https://github.com/user-attachments/assets/6c69319e-af16-468b-bc23-5a16e8268dd8" />



### Admin Dashboard

<img width="958" height="473" alt="image" src="https://github.com/user-attachments/assets/025f5d36-16bf-4605-98d9-7fbef10a6a1f" />
<img width="959" height="458" alt="image" src="https://github.com/user-attachments/assets/3f43cd82-9b29-4a01-bd70-bfa139ec8e69" />
<img width="953" height="365" alt="image" src="https://github.com/user-attachments/assets/edc5b875-f355-4dc2-9e92-b3b5e1876cc2" />
<img width="947" height="443" alt="image" src="https://github.com/user-attachments/assets/df114e10-4084-4044-bac0-2c39d1506c82" />





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
