# EcoLearn - Gamified Environmental Education Platform

Welcome to the **EcoLearn** project repository. This is an interactive, full-stack educational platform dedicated to teaching environmental topics through gamification, real-time engagement, and AI-driven experiences.

## 🚀 Features

- **Gamified Learning:** Explore interactive lessons, overcome challenges, take quizzes, and earn badges to track your progress and stay motivated.
- **Role-Based Access:** Distinct customized portals and dashboards for:
  - **Students:** Learning modules, quiz taking, and progress tracking.
  - **Teachers:** Content creation, student monitoring, and classroom administration.
  - **Admins:** Platform management, analytics, and user moderation.
- **Real-Time Interactions:** Live updates and real-time notifications via WebSockets.
- **AI-Powered:** Integrated with Google Generative AI to provide smart recommendations, dynamic quiz generation, and personalized learning assistance.
- **Rich Dashboard Analytics:** Dynamic charts and progressive stats visualization using Recharts.

## 💻 Tech Stack

### Frontend
- **Framework:** Next.js 16, React 19
- **Styling:** Tailwind CSS, Framer Motion for smooth animations, Lucide React for modern iconography
- **State/Real-time:** Socket.io-client, Axios
- **Data Visualization:** Recharts

### Backend
- **Framework:** Node.js, Express.js
- **Database:** MongoDB (via Mongoose)
- **Authentication:** JWT (JSON Web Tokens), bcryptjs
- **Real-time:** Socket.io
- **AI Integration:** `@google/generative-ai`
- **Other Utilities:** Nodemailer for email communications, dotenv, cors

## 📁 Project Structure

```
SGP-6/
├── frontend/       # Next.js web application
├── backend/        # Node.js/Express API server
├── database/       # Database scripts and configuration
├── Photos/         # Assets and images for the main project
└── ...             # Various utility scripts (e.g., set up environment)
```

## 🛠️ Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- MongoDB instance (Atlas or local)

### Environment Variables
You'll need to set up your environment variables for both the frontend and backend. Check `.env` inside the `backend` folder and `.env.local` inside the `frontend` folder. Make sure to define:
- `MONGO_URI`
- `JWT_SECRET`
- `GEMINI_API_KEY` (For AI functionalities)
- Email config (SMTP)

### Running the Backend
1. Navigate to the `backend` directory.
   ```bash
   cd backend
   ```
2. Install dependencies.
   ```bash
   npm install
   ```
3. Start the development server. (It uses dynamic port assignment but defaults to `3001`).
   ```bash
   npm run dev
   ```

### Running the Frontend
1. Navigate to the `frontend` directory.
   ```bash
   cd frontend
   ```
2. Install dependencies.
   ```bash
   npm install
   ```
3. Start the Next.js development server.
   ```bash
   npm run dev
   ```
4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📄 License
This project is part of an academic requirement (SEM6-SGP-70-75). 
