# Imagify - AI Image Generator

Imagify is a full-stack, modern web application that leverages artificial intelligence to generate stunning images. Built using the MERN stack, the platform incorporates a sleek frontend with fluid animations, seamless user authentication, and a credit-based system featuring Razorpay integration for payments.

## 🚀 Features

- **AI Image Generation:** Generate high-quality, creative images based on text prompts.
- **Secure Authentication:** User login and registration powered by JWT (JSON Web Tokens) and bcrypt password hashing.
- **Credit System & Payments:** Integrated with Razorpay so users can purchase credits to continue generating images seamlessly.
- **Beautiful & Responsive UI:** Built with React, Tailwind CSS, and Framer Motion for interactive micro-animations.
- **Robust Backend:** A scalable Express and Node.js server seamlessly connecting with MongoDB via Mongoose.

## 🛠️ Tech Stack

### Frontend (Client)
- **Framework:** React 19 / Vite
- **Routing:** React Router v7
- **Styling:** Tailwind CSS (with PostCSS & Autoprefixer)
- **Animations:** Framer Motion (`motion`)
- **Notifications:** React Toastify
- **HTTP Client:** Axios

### Backend (Server)
- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB & Mongoose
- **Authentication:** JSON Web Tokens (jsonwebtoken), bcrypt
- **Payments:** Razorpay
- **HTTP Client:** Axios & Form-Data 

## ⚙️ Installation & Setup

### Prerequisites
Make sure you have Node.js and npm installed. You will also need a MongoDB database (local or Atlas) and API keys for Razorpay and your chosen AI image generation provider.

### 1. Clone the repository
```bash
git clone https://github.com/rakshanrk/imagify-image-generator.git
cd imagify-image-generator
```

### 2. Setup the Backend
Navigate to the `server` directory, install dependencies, and setup the environment.

```bash
cd server
npm install
```

Create a `.env` file in the `server` directory and add the following keys:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
# Add your AI image generation API keys here based on the provider you used
```

Start the backend development server:
```bash
npm run server
```

### 3. Setup the Frontend
Open a new terminal session, navigate to the `client` directory, install dependencies, and start the Vite development server.

```bash
cd client
npm install
```

Create a `.env` file in the `client` directory:
```env
VITE_BACKEND_URL=http://localhost:5000
# Add your Razorpay key or any other client-side variables
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

Start the frontend development server:
```bash
npm run dev
```

## 📜 License
This project is open-source and available under the ISC License.
