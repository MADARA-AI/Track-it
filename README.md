# 🚀 TrackIt - Career Learning & Roadmap Platform

TrackIt is a comprehensive full-stack educational platform designed to help professionals and students navigate their career paths. It provides curated learning roadmaps, interactive courses, and personalized recommendations to streamline the journey from beginner to expert.

![License](https://img.shields.io/github/license/MADARA-AI/web-backend-bridge)
![JavaScript](https://img.shields.io/badge/language-JavaScript-yellow)
![React](https://img.shields.io/badge/frontend-React-blue)
![Express](https://img.shields.io/badge/backend-Express-lightgrey)
![MongoDB](https://img.shields.io/badge/database-MongoDB-green)

---

## ✨ Key Features

- **🗺️ Interactive Roadmaps**: Visual guides for various domains including Web Development and OSINT (Open Source Intelligence).
- **📚 Course Catalog**: A library of structured courses with difficulty levels, durations, and instructor details.
- **🎯 Career Recommendations**: AI-driven or rule-based suggestions to help users choose their next learning milestone.
- **🔐 Secure Authentication**: Complete user management system including Sign Up, Login, Password Reset, and Code Verification.
- **👤 User Profiles**: Personalized dashboards to track progress and manage account settings.
- **💳 Integrated Checkout**: Secure payment processing for premium courses via PayPal.
- **🔍 Global Search**: Find tools, courses, and roadmap nodes easily across the platform.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: [React](https://react.dev/) (v18/v19)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/), [Styled Components](https://styled-components.com/), [shadcn/ui](https://ui.shadcn.com/)
- **State Management**: [TanStack Query](https://tanstack.com/query/latest)
- **Routing**: [React Router Dom](https://reactrouter.com/)
- **Icons**: [Lucide React](https://lucide.dev/), [React Icons](https://react-icons.github.io/react-icons/)

### Backend
- **Runtime**: [Node.js](https://nodejs.org/) / [Bun](https://bun.sh/)
- **Server**: [Express.js](https://expressjs.com/)
- **Database**: [MongoDB](https://www.mongodb.com/) via [Mongoose](https://mongoosejs.com/)
- **Middleware**: CORS, JSON Parsing

---

## 📂 Project Structure

```text
├── client/              # React frontend (CRA bootstrapped)
│   ├── src/
│   │   ├── components/  # Reusable UI components (Auth, Pages, etc.)
│   │   ├── Style/       # CSS and styling files
│   │   └── App.js       # Main routing logic
├── server/              # Express backend
│   ├── models/          # Mongoose schemas (User, etc.)
│   ├── routes/          # API endpoints
│   ├── DB/              # Database connection logic
│   └── server.js        # Entry point
├── src/                 # Root-level Vite/Shadcn components (if applicable)
└── package.json         # Workspace configuration
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- MongoDB account (Atlas or Local)
- Bun (optional, but recommended for root tasks)

### 1. Clone the Repository
```bash
git clone https://github.com/MADARA-AI/web-backend-bridge.git
cd web-backend-bridge
```

### 2. Setup the Server
```bash
cd server
npm install
```
Create a `.env` file in the `server` directory:
```env
PORT=5000
DB=your_mongodb_connection_string
```
Start the server:
```bash
npm start
```

### 3. Setup the Client
```bash
cd ../client
npm install
npm start
```

The application should now be running at `http://localhost:3000`.

---

## 🔧 Environment Variables

The server requires the following variables to function correctly:

| Variable | Description | Default |
|----------|-------------|---------|
| `PORT`   | Port the server runs on | `5000` |
| `DB`     | MongoDB Connection String | `REQUIRED` |

---

## 🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

Distributed under the ISC License. See `LICENSE` for more information.

---

## 👤 Author

**MADARA-AI**
- GitHub: [@MADARA-AI](https://github.com/MADARA-AI)

*Developed with ❤️ as part of the TrackIt Learning ecosystem.*
