# 🌍 EnglishQazaq - Online English Learning Platform

**EnglishQazaq** is a comprehensive, production-ready SaaS platform for teaching English to Kazakh speakers. Built with modern technologies: Next.js, React, TypeScript, Tailwind CSS, Node.js, PostgreSQL, and Prisma.

## 🎯 Platform Features

### 📚 Learning System
- **Alphabet & Phonetics** - Interactive A-Z with pronunciation
- **1000+ Vocabulary** - English words with Kazakh translations, transcriptions, audio, examples
- **Grammar Courses** - 15+ comprehensive lessons (To Be, Present Simple, Past Simple, Future Simple, Modal Verbs, Articles, Prepositions, Passive Voice, etc.)
- **Interactive Exercises** - Multiple choice, fill-in-the-blanks, drag & drop, translation tasks

### 🎤 Speaking & Listening
- **Speech Recognition** - Web Speech API integration
- **Pronunciation Scoring** - Real-time feedback
- **Listening Tasks** - Audio exercises with validation

### ✍️ Writing & AI
- **Essay Writing** - User submissions and storage
- **AI Tutor** - GPT-powered assistant in Kazakh language
- **Grammar Checking** - Automatic error detection and suggestions
- **Conversational AI** - Dialog practice with AI

### 🎮 Gamification
- **XP System** - Points for completing tasks
- **Levels & Badges** - Progress tracking
- **Achievements** - Unlockable rewards
- **Daily/Weekly Challenges** - Streaks and bonuses
- **Leaderboard** - Global rankings

### 👤 User Features
- **Email & Google Authentication** - JWT-based security
- **User Profile** - Customization and statistics
- **Progress Tracking** - Detailed analytics
- **Certificate System** - PDF certificates with QR codes

### 💳 Monetization
- **Free Plan** - Limited features
- **Premium Plan** - Full course access
- **VIP Plan** - AI tutor + advanced features
- **Stripe Integration** - Secure payments

### 🔐 Admin Panel
- **Course Management** - Create, edit, delete lessons
- **User Management** - Monitor and manage users
- **Analytics Dashboard** - Statistics and insights
- **Payment Management** - Transaction tracking

---

## 🛠️ Tech Stack

### Frontend
- **Next.js 14+** - React framework
- **React 18+** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **React Query** - Data fetching
- **Zustand** - State management
- **next-auth** - Authentication

### Backend
- **Node.js** - Runtime
- **Next.js API Routes** - Backend endpoints
- **Express Middleware** - Request handling
- **JWT** - Authentication tokens
- **OpenAI/Groq API** - AI services

### Database & ORM
- **PostgreSQL** - Database
- **Prisma** - ORM with migrations
- **Redis** (optional) - Caching

### DevOps & Deployment
- **Docker** - Containerization
- **Docker Compose** - Multi-service orchestration
- **Vercel** - Frontend deployment
- **Railway/Render** - Backend deployment

### Security
- **bcrypt** - Password hashing
- **JWT** - Token-based auth
- **Rate Limiting** - DDoS protection
- **CORS** - Cross-origin security
- **CSRF Protection** - Token validation
- **Input Validation** - Zod schemas

---

## 📦 Project Structure

```
EnglishQazaq/
├── src/
│   ├── app/
│   │   ├── (auth)/
│   │   │   ├── login/page.tsx
│   │   │   ├── signup/page.tsx
│   │   │   └── reset-password/page.tsx
│   │   ├── (dashboard)/
│   │   │   ├── layout.tsx
│   │   │   ├── overview/page.tsx
│   │   │   ├── courses/page.tsx
│   │   │   ├── progress/page.tsx
│   │   │   └── profile/page.tsx
│   │   ├── (admin)/
│   │   │   ├── admin/page.tsx
│   │   │   ├── admin/users/page.tsx
│   │   │   ├── admin/courses/page.tsx
│   │   │   └── admin/analytics/page.tsx
│   │   ├── api/
│   │   │   ├── auth/
│   │   │   ├── users/
│   │   │   ├── courses/
│   │   │   ├── exercises/
│   │   │   └── payments/
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── components/
│   │   ├── auth/
│   │   ├── dashboard/
│   │   ├── courses/
│   │   ├── exercises/
│   │   ├── ui/
│   │   └── admin/
│   ├── lib/
│   │   ├── auth.ts
│   │   ├── db.ts
│   │   ├── api-client.ts
│   │   └── utils.ts
│   ├── hooks/
│   │   ├── useAuth.ts
│   │   ├── useCourses.ts
│   │   └── useUser.ts
│   ├── types/
│   │   ├── index.ts
│   │   └── api.ts
│   ├── styles/
│   │   └── globals.css
│   └── middleware.ts
├── prisma/
│   ├── schema.prisma
│   └── seed.ts
├── public/
│   ├── fonts/
│   ├── images/
│   └── icons/
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── docs/
│   ├── SETUP.md
│   ├── API.md
│   └── DATABASE.md
├── .env.example
├── next.config.js
├── tsconfig.json
├── tailwind.config.js
├── postcss.config.js
└── package.json
```

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- PostgreSQL 14+
- npm or yarn

### Installation

```bash
# Clone repository
git clone https://github.com/bauirjanlesbek-hash/EnglishQazaq.git
cd EnglishQazaq

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env.local

# Setup database
npx prisma migrate dev --name init
npx prisma db seed

# Run development server
npm run dev
```

### Access
- Frontend: http://localhost:3000
- Admin Panel: http://localhost:3000/admin
- Database UI: http://localhost:5555 (Prisma Studio)

---

## 📖 Documentation

See detailed documentation:
- [Setup Guide](./docs/SETUP.md)
- [API Documentation](./docs/API.md)
- [Database Schema](./docs/DATABASE.md)

---

## 🔐 Security Features

✅ JWT Authentication
✅ OAuth 2.0 (Google)
✅ Rate Limiting
✅ CSRF Protection
✅ XSS Prevention
✅ SQL Injection Prevention
✅ Password Hashing (bcrypt)
✅ CORS Configuration
✅ Helmet.js (Security Headers)

---

## 💰 Pricing Plans

### Free
- 50 lessons
- 500 vocabulary words
- Limited exercises
- No AI tutor

### Premium ($9.99/month)
- All lessons (1000+)
- Full vocabulary
- Unlimited exercises
- AI tutor (limited)
- Certificate

### VIP ($19.99/month)
- Everything in Premium
- Unlimited AI tutor
- Advanced speaking features
- Priority support
- Custom learning path

---

## 🤝 Contributing

Contributions are welcome! Please read our Contributing Guidelines.

---

## 📄 License

This project is licensed under the MIT License.

---

## 📧 Support

For questions or issues, please contact: support@englishqazaq.com

---

**Made with ❤️ by EnglishQazaq Team**