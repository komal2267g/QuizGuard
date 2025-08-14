# QuizGuard 🛡️

![QuizGuard Screenshot](public/screenshot.png) <!-- Replace with your actual screenshot path -->

[![CI/CD](https://github.com/komal2267g/QuizGuard/actions/workflows/deploy.yml/badge.svg)](https://github.com/komal2267g/QuizGuard/actions)
![Node.js](https://img.shields.io/badge/node-%3E%3D20-brightgreen)
![Docker](https://img.shields.io/badge/docker-ready-blue)

🔗 **Live Demo:** [https://quizguard-p5t8.onrender.com](https://quizguard-p5t8.onrender.com)

---

## 📌 Overview
QuizGuard is a secure online quiz platform with **role-based access** for Teachers and Students, built to prevent cheating and ensure fair assessments.

---

## 🚀 Features

**Admin (Teacher)**
- Create quizzes with custom questions.
- Generate unique access links.
- View & download student scores (PDF).
- Dashboard with all submissions.

**Student**
- Join via unique link, enter roll number & name.
- Full-screen enforced quiz mode.
- Tab-switch warning & quit option.
- Instant confirmation email with score.

---

## 🛠 Tech Stack
- **Frontend:** React + TypeScript + Tailwind CSS + Vite
- **Backend/DB:** Supabase
- **Build:** Docker, Nginx
- **CI/CD:** GitHub Actions → Render
- **Security Scan:** Trivy

---

## ⚡ Quick Start

```bash
# Clone the repository
git clone https://github.com/komal2267g/QuizGuard.git
cd QuizGuard

# Install dependencies
npm ci

# Run locally
npm run dev

🐳 Docker Build
docker build -t quizguard-frontend -f Dockerfile.frontend .
docker-compose up

🔄 CI/CD

Push to main → GitHub Actions builds & deploys to Render.

Deployment URL: https://quizguard-p5t8.onrender.com