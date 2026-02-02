# 🚀 TrackIt - Career Learning & Roadmap Platform

> A modern, full-stack educational platform for career development and skill tracking

TrackIt is a comprehensive educational platform that empowers professionals and students to navigate their career paths effectively. Built with modern web technologies, it offers curated learning roadmaps, interactive courses, and personalized recommendations to streamline the journey from beginner to expert.

[![License](https://img.shields.io/github/license/MADARA-AI/web-backend-bridge)](LICENSE)
[![React](https://img.shields.io/badge/React-18.3.1-61DAFB?logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-3178C6?logo=typescript)](https://www.typescriptlang.org/)
[![Express](https://img.shields.io/badge/Express-4.x-000000?logo=express)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-6.x-47A248?logo=mongodb)](https://www.mongodb.com/)
[![Vite](https://img.shields.io/badge/Vite-5.4.1-646CFF?logo=vite)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4.11-06B6D4?logo=tailwindcss)](https://tailwindcss.com/)

**Live Demo:** [Coming Soon]  
**Documentation:** [Wiki](https://github.com/MADARA-AI/web-backend-bridge/wiki)

---

## 📸 Screenshots

<details>
<summary>Click to view screenshots</summary>

> Screenshots and demo GIFs will be added here

</details>

---

## ✨ Key Features

### Core Functionality
- **🗺️ Interactive Roadmaps**: Visual, node-based guides for career paths including Web Development, OSINT (Open Source Intelligence), and more
- **📚 Course Catalog**: Comprehensive library of structured courses with:
  - Difficulty level indicators (Beginner, Intermediate, Advanced)
  - Duration estimates and time commitments
  - Instructor profiles and credentials
  - Prerequisites and learning outcomes
- **🎯 Career Recommendations**: Intelligent suggestion engine to guide users toward their next learning milestone
- **🔍 Global Search**: Fast, full-text search across courses, roadmaps, and resources

### User Management
- **🔐 Secure Authentication**: Complete user management system with:
  - User registration and login
  - Password reset with email verification
  - Multi-factor authentication support
  - Session management
- **👤 User Profiles**: Personalized dashboards featuring:
  - Progress tracking and analytics
  - Course completion history
  - Saved roadmaps and bookmarks
  - Account settings management

### Commerce
- **💳 Integrated Checkout**: Secure payment processing for premium content via PayPal integration

---

## 🏗️ Architecture Overview

TrackIt follows a modern, decoupled architecture pattern:

```
┌─────────────────────────────────────────────────────────┐
│                      Frontend (React)                    │
│  • Vite Build Tool                                       │
│  • React Router for SPA Navigation                       │
│  • TanStack Query for Server State                       │
│  • Shadcn/UI + Tailwind CSS for Styling                  │
└──────────────────┬──────────────────────────────────────┘
                   │
                   │ REST API
                   │
┌──────────────────▼──────────────────────────────────────┐
│                  Backend (Express.js)                    │
│  • RESTful API Endpoints                                 │
│  • JWT Authentication                                    │
│  • Mongoose ODM                                          │
└──────────────────┬──────────────────────────────────────┘
                   │
                   │ MongoDB Driver
                   │
┌──────────────────▼──────────────────────────────────────┐
│                  Database (MongoDB)                      │
│  • User Collections                                      │
│  • Course & Roadmap Data                                 │
│  • Session Storage                                       │
└─────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: [React](https://react.dev/) 18.3.1 with TypeScript
- **Build Tool**: [Vite](https://vitejs.dev/) 5.4.1 for fast HMR and optimized builds
- **Styling**: 
  - [Tailwind CSS](https://tailwindcss.com/) 3.4.11 for utility-first styling
  - [Shadcn/UI](https://ui.shadcn.com/) component library
  - [Radix UI](https://www.radix-ui.com/) primitives
- **State Management**: 
  - [TanStack Query](https://tanstack.com/query/latest) v5 for server state
  - [React Hook Form](https://react-hook-form.com/) for form state
- **Routing**: [React Router Dom](https://reactrouter.com/) v6
- **Icons**: [Lucide React](https://lucide.dev/)
- **Form Validation**: [Zod](https://zod.dev/) schemas

### Backend
- **Runtime**: [Node.js](https://nodejs.org/) (v18+) / [Bun](https://bun.sh/)
- **Framework**: [Express.js](https://expressjs.com/) 4.x
- **Database**: [MongoDB](https://www.mongodb.com/) with [Mongoose](https://mongoosejs.com/) ODM
- **Authentication**: JWT-based authentication
- **Middleware**: 
  - CORS for cross-origin requests
  - Express JSON parser
  - Custom error handling

### Development Tools
- **Package Manager**: npm / bun
- **Linting**: ESLint with TypeScript support
- **Version Control**: Git & GitHub

---

## 📂 Project Structure

```text
web-backend-bridge/
├── client/                 # Legacy React frontend (CRA)
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── Style/          # CSS and styling files
│   │   └── App.js          # Main routing logic
│   └── package.json
│
├── server/                 # Express.js backend
│   ├── models/             # Mongoose schemas (User, Course, etc.)
│   ├── routes/             # API endpoint definitions
│   │   └── userRoutes.js   # User authentication & management
│   ├── DB/                 # Database connection configuration
│   ├── server.js           # Entry point
│   └── package.json
│
├── src/                    # Main Vite/React application (TypeScript)
│   ├── components/         # Shadcn/UI components
│   │   └── ui/             # Base UI components
│   ├── pages/              # Route page components
│   │   ├── Index.tsx       # Landing page
│   │   └── NotFound.tsx    # 404 page
│   ├── hooks/              # Custom React hooks
│   ├── lib/                # Utility functions and helpers
│   ├── App.tsx             # Main app component
│   └── main.tsx            # Vite entry point
│
├── public/                 # Static assets
├── vite.config.ts          # Vite configuration
├── tailwind.config.ts      # Tailwind CSS configuration
├── tsconfig.json           # TypeScript configuration
├── package.json            # Root workspace configuration
└── README.md               # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed on your system:
- **Node.js** (v18 or higher) - [Download](https://nodejs.org/)
- **npm** (comes with Node.js) or **bun** (optional) - [Download Bun](https://bun.sh/)
- **MongoDB** account (MongoDB Atlas recommended) - [Sign Up](https://www.mongodb.com/cloud/atlas)
- **Git** - [Download](https://git-scm.com/)

### Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/MADARA-AI/web-backend-bridge.git
cd web-backend-bridge
```

#### 2. Setup the Backend Server
```bash
cd server
npm install
```

Create a `.env` file in the `server` directory:
```env
# Server Configuration
PORT=5000

# Database
DB=mongodb+srv://username:password@cluster.mongodb.net/trackit?retryWrites=true&w=majority

# Authentication (Optional - if JWT is implemented)
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRE=7d

# Email Service (Optional - for password reset)
EMAIL_SERVICE=gmail
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-email-password
```

Start the backend server:
```bash
npm start
# Server will run on http://localhost:5000
```

#### 3. Setup the Frontend Application
Open a new terminal window:

```bash
cd web-backend-bridge  # Go back to root
npm install
```

Start the development server:
```bash
npm run dev
# Application will run on http://localhost:5173
```

#### 4. (Optional) Setup Legacy Client
If you want to run the legacy client:
```bash
cd client
npm install
npm start
# Legacy client will run on http://localhost:3000
```

### Quick Start with Bun

If you have Bun installed, you can use it for faster dependency installation:

```bash
# Install dependencies with Bun
bun install

# Run development server
bun run dev
```

---

## 🔧 Configuration

### Environment Variables

#### Backend Server (`server/.env`)

| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| `PORT` | Port the server runs on | No | `5000` |
| `DB` | MongoDB Connection String | **Yes** | - |
| `JWT_SECRET` | Secret key for JWT tokens | Recommended | - |
| `JWT_EXPIRE` | JWT expiration time | No | `7d` |
| `EMAIL_SERVICE` | Email service provider | No | - |
| `EMAIL_USER` | Email account username | No | - |
| `EMAIL_PASS` | Email account password | No | - |

#### Frontend Application

The frontend uses Vite environment variables. Create a `.env` file in the root directory:

```env
# API Configuration
VITE_API_URL=http://localhost:5000

# Feature Flags
VITE_ENABLE_ANALYTICS=false
```

---

## 📡 API Documentation

### Base URL
```
http://localhost:5000
```

### Endpoints

#### Authentication

```http
POST /api/users/register
Content-Type: application/json

{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "securePassword123"
}
```

```http
POST /api/users/login
Content-Type: application/json

{
  "email": "john@example.com",
  "password": "securePassword123"
}
```

#### User Management

```http
GET /api/users/profile
Authorization: Bearer {token}
```

```http
PUT /api/users/profile
Authorization: Bearer {token}
Content-Type: application/json

{
  "name": "John Updated",
  "bio": "Full-stack developer"
}
```

> 📚 For complete API documentation, visit the [API Wiki](https://github.com/MADARA-AI/web-backend-bridge/wiki/API-Documentation)

---

## 🧪 Testing

### Running Tests

```bash
# Run all tests
npm test

# Run tests with coverage
npm run test:coverage

# Run tests in watch mode
npm run test:watch
```

### Test Structure

```
server/
└── __tests__/
    ├── unit/
    │   ├── models/
    │   └── utils/
    └── integration/
        └── routes/
```

---

## 🚢 Deployment

### Backend Deployment (Heroku Example)

```bash
# Install Heroku CLI
npm install -g heroku

# Login to Heroku
heroku login

# Create a new Heroku app
cd server
heroku create trackit-backend

# Set environment variables
heroku config:set DB=your_mongodb_connection_string
heroku config:set JWT_SECRET=your_secret

# Deploy
git push heroku main
```

### Frontend Deployment (Vercel Example)

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
cd web-backend-bridge
vercel

# Set environment variables in Vercel dashboard
# VITE_API_URL=https://your-backend-url.herokuapp.com
```

### Alternative Deployment Options

- **Frontend**: Netlify, Vercel, GitHub Pages, Cloudflare Pages
- **Backend**: Heroku, Railway, Render, AWS EC2, DigitalOcean
- **Database**: MongoDB Atlas (recommended), AWS DocumentDB

---

## 🧑‍💻 Development

### Available Scripts

#### Root Directory
```bash
npm run dev          # Start Vite development server
npm run build        # Build for production
npm run build:dev    # Build in development mode
npm run preview      # Preview production build
npm run lint         # Run ESLint
```

#### Server Directory
```bash
npm start            # Start Express server
npm run dev          # Start with nodemon (auto-reload)
npm test             # Run tests
```

### Code Style

This project uses ESLint for code quality. Configuration is in `eslint.config.js`.

```bash
# Check for linting errors
npm run lint

# Auto-fix linting errors
npm run lint -- --fix
```

### Git Workflow

1. Create a feature branch: `git checkout -b feature/amazing-feature`
2. Make your changes and commit: `git commit -m 'Add amazing feature'`
3. Push to the branch: `git push origin feature/amazing-feature`
4. Open a Pull Request

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### How to Contribute

1. **Fork the Repository**
   - Click the "Fork" button at the top right of this page

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/your-username/web-backend-bridge.git
   cd web-backend-bridge
   ```

3. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-amazing-feature
   ```

4. **Make Your Changes**
   - Write clear, commented code
   - Follow the existing code style
   - Add tests if applicable

5. **Commit Your Changes**
   ```bash
   git add .
   git commit -m 'feat: add amazing feature'
   ```
   
   Use [Conventional Commits](https://www.conventionalcommits.org/) format:
   - `feat:` for new features
   - `fix:` for bug fixes
   - `docs:` for documentation changes
   - `style:` for formatting changes
   - `refactor:` for code refactoring
   - `test:` for adding tests
   - `chore:` for maintenance tasks

6. **Push to Your Fork**
   ```bash
   git push origin feature/your-amazing-feature
   ```

7. **Open a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your feature branch
   - Fill out the PR template
   - Wait for review

### Development Guidelines

- **Code Quality**: Ensure your code passes all linting checks
- **Testing**: Add tests for new features
- **Documentation**: Update documentation for any API changes
- **Commit Messages**: Use clear, descriptive commit messages
- **Pull Requests**: Keep PRs focused and small

### Reporting Bugs

Found a bug? Please open an issue with:
- A clear title and description
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Your environment (OS, Node version, etc.)

---

## 📋 Roadmap

- [ ] Add comprehensive test coverage (unit & integration tests)
- [ ] Implement real-time notifications using WebSockets
- [ ] Add progress analytics and visualization dashboard
- [ ] Implement social features (user connections, sharing)
- [ ] Add mobile application (React Native)
- [ ] Integrate more payment providers
- [ ] Add AI-powered course recommendations
- [ ] Implement dark mode theme
- [ ] Add internationalization (i18n) support
- [ ] Create admin dashboard for content management

---

## 🐛 Known Issues

- Legacy client (CRA) is deprecated in favor of the new Vite application
- Some API endpoints may need authentication middleware updates
- Email service configuration is currently optional

---

## 📄 License

This project is licensed under the **ISC License** - see the [LICENSE](LICENSE) file for details.

```
ISC License

Copyright (c) 2024 MADARA-AI

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.
```

---

## 👥 Authors & Acknowledgments

### Core Team

**MADARA-AI** - *Lead Developer & Project Maintainer*
- GitHub: [@MADARA-AI](https://github.com/MADARA-AI)
- Email: [Available on request]

### Acknowledgments

- Built with [React](https://react.dev/) and [Express.js](https://expressjs.com/)
- UI components from [Shadcn/UI](https://ui.shadcn.com/)
- Icons from [Lucide](https://lucide.dev/)
- Inspired by [Roadmap.sh](https://roadmap.sh/) and other learning platforms

### Contributors

Thanks to all contributors who have helped improve this project!

<!-- ALL-CONTRIBUTORS-LIST:START -->
<!-- Add contributors here -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

---

## 📞 Support & Contact

- **Issues**: [GitHub Issues](https://github.com/MADARA-AI/web-backend-bridge/issues)
- **Discussions**: [GitHub Discussions](https://github.com/MADARA-AI/web-backend-bridge/discussions)
- **Documentation**: [Wiki](https://github.com/MADARA-AI/web-backend-bridge/wiki)

---

## ⭐ Show Your Support

If you find this project helpful, please consider giving it a star on GitHub! It helps others discover the project and motivates further development.

---

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/MADARA-AI/web-backend-bridge?style=social)
![GitHub forks](https://img.shields.io/github/forks/MADARA-AI/web-backend-bridge?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/MADARA-AI/web-backend-bridge?style=social)

---

<div align="center">
  
**Built with ❤️ by MADARA-AI**

*Empowering learners to achieve their career goals through structured, accessible education*

[⬆ Back to Top](#-trackit---career-learning--roadmap-platform)

</div>
