# 🎓 LimbusMentor

**AI-Powered Adaptive Learning Platform**

LimbusMentor is an intelligent study companion that generates customized learning materials and adaptive quizzes using AI. Guided by Limbus, your eternal scholar, it helps students master any subject through personalized summaries and comprehensive testing, visit Limbus's temple [here](https://limbus-mentor.up.railway.app)

![LimbusMentor](./src/assets/limbus-mentor.jpg)

---

## ✨ Features

### 🧠 AI-Powered Learning
- **Intelligent Summaries**: Generate comprehensive study materials on any topic using OpenAI
- **Adaptive Difficulty**: Choose from Simple, Normal, or Advanced learning levels
- **Personalized Quizzes**: AI-generated questions tailored to your chosen subject and difficulty

### 🌍 Multilingual Support
- **Full Internationalization**: Complete support for English and Bulgarian
- **Seamless Switching**: Toggle between languages with persistent preferences

### 📊 Progress Tracking
- **Detailed History**: View all past study sessions and quiz results
- **Performance Analytics**: Track your scores and improvement over time
- **Visual Charts**: Interactive graphs showing your learning journey

### 🎨 Beautiful UI/UX
- **Modern Design**: Clean, gradient-rich interface with smooth animations
- **Dark/Light Themes**: Persistent theme preference across sessions
- **Responsive**: Fully optimized for desktop and mobile devices
- **Character-Driven**: Featuring Limbus, your AI mentor companion

---

## 🏗️ Architecture

LimbusMentor uses a modern full-stack architecture deployed on Railway:

```
┌─────────────────────┐         ┌──────────────────────┐
│   Frontend (React)  │ ◄─────► │  Backend (FastAPI)   │
│  Railway Hosted     │  HTTPS  │   Railway Hosted     │
│  Vite + TypeScript  │         │   PostgreSQL DB      │
└─────────────────────┘         └──────────────────────┘
         │                                  │
         │                                  │
         └──────────────┬───────────────────┘
                        │
                   OpenAI API
```

### Frontend
- **Host**: Railway 
- **Framework**: React 18 + TypeScript
- **Build Tool**: Vite
- **UI Library**: shadcn/ui + Radix UI
- **Styling**: Tailwind CSS with custom design system
- **State Management**: React Context API + TanStack Query

### Backend
- **Host**: Railway 
- **Framework**: FastAPI (Python)
- **Database**: PostgreSQL
- **ORM**: SQLAlchemy
- **Authentication**: JWT tokens
- **AI Integration**: Grok API

---

## 🔒 Security

- **Password Hashing**: All passwords are hashed using bcrypt
- **JWT Authentication**: Secure token-based authentication
- **Input Validation**: Comprehensive validation using Pydantic and Zod
- **CORS Protection**: Configured CORS policies
- **Environment Variables**: Sensitive data stored securely

---

## 🌟 Key Features Explained

### Adaptive Learning System
The AI analyzes your chosen subject and difficulty level to generate:
- Structured summaries with key concepts
- Progressive explanations from fundamentals to advanced topics
- Contextual examples and applications

### Quiz Generation
- Multiple-choice questions tailored to your study material
- Difficulty-appropriate questions
- Instant feedback and scoring
- Detailed result tracking

### Progress Analytics
- Historical performance tracking
- Visual charts showing improvement
- Session-based organization
- Score percentages and time tracking

---


## 🙏 Acknowledgments

- **Limbus Character**: The AI mentor mascot guiding the learning experience
- **OpenAI**: For GPT-4 API powering the AI features
- **shadcn/ui**: For the beautiful component library
- **Railway**: For hosting infrastructure

---


