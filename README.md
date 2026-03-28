# 🚀 AI Interview Analyzer (Next.js + OpenAI + Supabase)

An intelligent, full-stack AI-powered interview platform that simulates real-world technical interviews, evaluates candidate responses, and provides actionable feedback using LLMs.

> Built for placement preparation with real-world system design and AI integration.

---

## 🌐 Live Demo

https://ai-interview-mocker-delta.vercel.app/

---

## 📦 GitHub Repository

👉 https://github.com/Ajendranath/Ai-Mock-Interview-Platform

---

## 🧠 Features

* 🤖 **AI Interview Generation**

  * Dynamic question generation based on role, skills, and experience
  * Powered by OpenAI (LLM)

* 🗣️ **Answer Evaluation**

  * AI analyzes user responses and gives:

    * Score
    * Strengths & weaknesses
    * Improvement suggestions

* 📊 **Interview Analytics Dashboard**

  * Track past interviews
  * Performance trends & scoring insights

* ⚡ **Real-Time Experience**

  * Smooth interaction with instant feedback
  * (Optional: WebSocket-based live interviewer mode)

* 🔐 **Authentication**

  * Secure login/signup using Supabase Auth

* 🗄️ **Database (PostgreSQL via Supabase)**

  * Stores:

    * Interview history
    * User responses
    * AI evaluations

---

## 🏗️ Tech Stack

### Frontend

* Next.js (React)
* Tailwind CSS

### Backend

* Node.js (Next.js API routes)
* REST APIs

### Database

* Supabase (PostgreSQL)

### AI Integration

* OpenAI API (GPT models)

### Other Tools

* Supabase Auth
* Vercel (Deployment)
* (Optional) Redis (rate limiting & caching)

---

## 📁 Project Structure

```
/app
/components
/lib
  ├── supabaseClient.js
  ├── openai.js
/pages/api
  ├── generate-questions.js
  ├── evaluate-answer.js
  ├── save-interview.js
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Ajendranath/Ai-Mock-Interview-Platform.git
cd Ai-Mock-Interview-Platform
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Setup environment variables

Create a `.env.local` file:

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_key
OPENAI_API_KEY=your_openai_key
```

---

### 4️⃣ Run locally

```bash
npm run dev
```

App runs at:

```
http://localhost:3000
```

---

## 📊 Database Schema (Supabase)

### Users

* id
* email

### Interviews

* id
* user_id
* role
* questions
* created_at

### Responses

* id
* interview_id
* question
* answer
* score
* feedback

---

## 🚀 Future Enhancements

* 🎤 Voice-based interview (speech-to-text)
* 📈 Advanced analytics (graphs & insights)
* 🤝 Peer interview mode (real-time WebSocket)
* 🧠 Embedding-based answer similarity scoring
* 💳 SaaS billing (Stripe integration)

---

## 💡 Why This Project?

This project demonstrates:

* Real-world **AI integration (LLMs)**
* Full-stack architecture (Next.js + APIs)
* Database design using PostgreSQL (Supabase)
* Scalable and modular backend structure
* Product thinking and user-centric design

---

## 🧑‍💻 Author

**Ajendra Nath Tripathi**
Final Year CSE Student | Aspiring Software Engineer

---

## ⭐ Contribute / Support

If you found this project useful:

* ⭐ Star the repo
* 🍴 Fork and improve
* 🛠️ Raise issues / PRs

---

## 📜 License

MIT License
