
---

```markdown
# 🗨️ Bantr Chat Application

**Bantr** is a full-stack, real-time web chat platform built with the *MERN* stack (MongoDB, Express, React, Node.js). It enables users to securely register, log in, manage profiles, and exchange instant messages and images. Designed for individuals, teams, and communities seeking a modern, responsive, and customizable chat experience.

🌐 **Live Demo**: [https://bantr-mern-chatapp-1.onrender.com](https://bantr-mern-chatapp-1.onrender.com)

---

## 📚 Table of Contents

- [Overview](#-bantr-chat-application)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Demo](#-live-demo)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Scripts](#-scripts)
- [Contributing](#-contributing)
- [License](#-license)

---

## ✨ Features

- 🔐 **Secure Authentication**  
  JWT-based login with HTTP-only cookies to protect sessions.

- 💬 **Real-Time Messaging**  
  Instant 1-on-1 messaging powered by *Socket.IO*, including online/offline presence indicators.

- 🖼️ **Image and Media Sharing**  
  Upload and send images directly in chat via *Cloudinary* integration.

- 👤 **User Profile Management**  
  Upload avatars, update profile data, and personalize your user identity.

- 🧑‍🤝‍🧑 **Responsive Sidebar Contacts**  
  View all available users (excluding self), with a toggle for “online only” filter.

- ⌨️ **Typing Indicators** *(Planned)*  
  Know when others are typing for more interactive conversations.

- 🎨 **Theming and Customization**  
  Toggle between dark/light modes and choose from a wide variety of *DaisyUI* themes.

- ⏳ **Loading Skeletons & Toasts**  
  Smooth UX with animated skeletons during data fetches and toast notifications.

- 📱 **Mobile-First Responsive Design**  
  Optimized for desktop, tablet, and mobile use.

- 📧 **Forgot Password Flow** *(Coming Soon)*  
  Secure password reset with email verification.

- 🛡️ **Rate Limiting & Security**  
  All backend endpoints protected via *express-rate-limit* and secure practices.

- 🧑‍💻 **Modern Developer Experience**  
  Fast builds via *Vite*, clean modular code, and separate client/server structure.

- 🛠️ **Planned Enhancements**  
  Group chats, message reactions, push notifications, advanced search/filtering.

---

## 🛠️ Tech Stack

### 🖥️ Client

- *React 19*, *Vite*
- *Tailwind CSS*, *DaisyUI*
- *Zustand*, *React Router v7*
- *Axios*, *react-hot-toast*, *lucide-react*
- *socket.io-client*

### ⚙️ Server

- *Node.js*, *Express.js*
- *MongoDB*, *Mongoose*
- *Socket.IO*, *JWT*, *bcryptjs*
- *Cloudinary*, *Nodemailer*
- *express-rate-limit*

### ☁️ DevOps & Deployment

- Docker (planned)
- Nginx (reverse proxy)
- AWS EC2 / Render

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/bantr.git
cd bantr
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the `backend/` directory (see [Environment Variables](#-environment-variables)).

### 4. (Optional) Seed the Database

```bash
cd backend
node src/seeds/user.seed.js
cd ..
```

### 5. Start Backend Server

```bash
npm run start
```

### 6. Start Frontend Dev Server

```bash
npm run dev --workspace frontend
```

### 7. Open in Browser

Visit [http://localhost:5173](http://localhost:5173) to use Bantr locally.

---

## 🔐 Environment Variables

Create a `.env` file inside the `backend/` directory with the following keys:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
EMAIL_USER=your_email_account
EMAIL_PASS=your_email_password
FRONTEND_URL=http://localhost:5173
NODE_ENV=development
```

---

## 💡 Usage

### 📝 Register or Login
- Sign up with an email and password or log in with an existing account.

### 👥 Select a Contact
- View users in the sidebar (excluding yourself).
- Filter to show only online contacts.

### 💬 Start Chatting
- Send real-time text messages instantly.
- Upload and send images within the chat.

### 👤 Manage Profile
- Update your avatar and profile info on the Profile page.

### 🎨 Switch Themes
- Go to **Settings** to choose between light, dark, or DaisyUI themes.

### 🔄 Forgot Password *(Coming Soon)*
- Use the “Forgot Password?” feature on the login page to reset credentials via email.

### 📱 Use Anywhere
- Mobile-friendly UI adapts to all screen sizes.

### 🔒 Logout Securely
- Click the **Logout** button in the Navbar to end your session.

> 💡 **Tip:** Use the latest browser version and a stable internet connection for the best experience.

---

## 🧱 Project Structure

```
bantr/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── lib/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   └── seeds/
│   ├── socket.js
│   └── index.js
├── frontend/
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── store/
│       ├── lib/
│       └── App.jsx
├── docker-compose.yml (planned)
└── README.md
```

---

## 🧪 Scripts

| Command                                  | Description                         |
|------------------------------------------|-------------------------------------|
| `npm run start`                          | Starts the backend server           |
| `npm run dev --workspace frontend`       | Starts the frontend dev server      |
| `npm run build`                          | Builds frontend and backend assets  |
| `npm run seed`                           | Seeds the database with test users  |

---

## 🤝 Contributing

We welcome community contributions!

1. **Fork** the repo
2. **Create** a new branch: `git checkout -b feature/your-feature`
3. **Commit** your changes: `git commit -m 'Add feature'`
4. **Push** to your branch: `git push origin feature/your-feature`
5. **Open a Pull Request**

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---


```

Let me know if you’d like this split into separate frontend/backend READMEs or if you want a Chinese version too!
