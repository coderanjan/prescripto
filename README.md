# 🏥 Prescripto

**Prescripto** is a doctor appointment booking platform that connects patients with doctors for easy scheduling, and gives admins tools to manage doctors, appointments, and platform data.

## 🔗 Live Links

| App | Link |
|---|---|
| 🌐 Patient Frontend | [prescripto-frontend-kok2.onrender.com](https://prescripto-frontend-kok2.onrender.com/) |
| 🛠️ Admin Panel | [prescripto-admin-tkj9.onrender.com](https://prescripto-admin-tkj9.onrender.com/) |
| 💻 Source Code | [github.com/coderanjan/prescripto](https://github.com/coderanjan/prescripto) |

> ⚠️ Since this app is hosted on Render's free tier, the first request after a period of inactivity may take **30–60 seconds** to load while the server spins back up.

## ✨ Features

- 👤 Patient registration and login
- 🩺 Browse doctors by specialty
- 📅 Book, reschedule, and cancel appointments
- 💳 Online payment for appointments
- 🖼️ Profile management with image upload
- 🔐 JWT-based authentication for patients, doctors, and admins
- 🛠️ Admin dashboard to add/manage doctors and view all appointments
- 📱 Fully responsive UI

## 🧰 Tech Stack

**Frontend & Admin Panel**
- React (Vite)
- React Router
- Tailwind CSS / CSS
- Axios
- Context API for state management

**Backend** 
- Node.js & Express.js
- MongoDB with Mongoose
- JSON Web Tokens (JWT) for authentication
- Multer / Cloudinary for image uploads
- Razorpay for payments

**Deployment**
- Render (Frontend, Admin & Backend)


## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or later)
- npm or yarn
- A running instance of the Prescripto backend API (and its `MONGODB_URI`, if you're running the full stack locally)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/coderanjan/prescripto.git
   cd prescripto
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   Create a `.env` file in the project root:

   ```env
   VITE_BACKEND_URL=http://localhost:4000
   ```

4. **Run the development server**

   ```bash
   npm run dev
   ```

   The app will be available at `http://localhost:5173`.

5. **Build for production**

   ```bash
   npm run build
   ```

## 🖥️ Admin Panel

The admin panel is a separate application used to manage doctors and appointments. It is deployed at [prescripto-admin-tkj9.onrender.com](https://prescripto-admin-tkj9.onrender.com/). Refer to its own setup instructions if it lives in a separate repository/folder.

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## 📄 License

This project is available under the [MIT License](LICENSE).

## 📬 Contact

Maintained by [@coderanjan](https://github.com/coderanjan). For questions or issues, please open an [issue](https://github.com/coderanjan/prescripto/issues) on GitHub.
