
# 🔥 Fullstack Starter Project — NestJS + Prisma + Next.JS

This is a fullstack starter boilerplate that combines a robust **NestJS backend** with **Prisma ORM** and a modern **frontend Next.js. It includes user authentication, protected API routes, and a clean structure to scale your applications efficiently.

---

## 🧱 Tech Stack

### Backend

- **NestJS** - Progressive Node.js backend framework
- **Prisma** - Type-safe ORM for PostgreSQL (or others)
- **JWT** - Authentication via JSON Web Tokens
- **bcrypt** - Password hashing
- **PostgreSQL** - Default DB (can be changed)
- **dotenv** - Environment variable management

### Frontend

- **Next.js / React** - Frontend framework (or any SPA)
- **Axios / Fetch** - API communication
- **JWT handling** - Frontend-side token storage and protection
- **TailwindCSS / Chakra UI** - UI styling (optional)

---

## 📂 Project Structure

```
project-root/
│
├── backend/               # NestJS backend
│   ├── src/
│   └── .env
│
├── frontend/              # Next.js or React frontend
│   ├── pages/             # Frontend routes
│   ├── components/        # Reusable UI elements
│   └── .env.local
│
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Geowar17/fullstack-nestjs-prisma.git
cd fullstack-nestjs-prisma
```

### 2. Setup Backend

```bash
cd backend
npm install
cp .env.example .env
# Update .env with your DB and JWT secret
npx prisma migrate dev --name init
npm run start:dev
```

Backend will run at: `http://localhost:3000`

### 3. Setup Frontend

```bash
cd ../frontend
npm install
cp .env.example .env.local
# Make sure it points to your backend base URL
npm run dev
```

Frontend will run at: `http://localhost:3001`

---

## 🔐 Auth Routes (Backend)

| Method | Endpoint     | Description           |
|--------|--------------|-----------------------|
| POST   | /auth/signup | Register a user       |
| POST   | /auth/login  | Login and get token   |
| GET    | /users/me    | Get logged-in profile |

---

## ✨ Features

- Modular and clean folder structure
- Full user authentication flow
- Protected frontend routes
- Prisma schema setup and migrations
- Scalable fullstack architecture

---

## 🔧 Environment Variables

### Backend `.env`

```
DATABASE_URL=postgresql://user:pass@localhost:5432/dbname
JWT_SECRET=your_jwt_secret
```

### Frontend `.env.local`

```
NEXT_PUBLIC_API_URL=http://localhost:3000
```

---

## 📦 Future Plans

- ⬜ Role-based access control
- ⬜ Email verification
- ⬜ Password reset via email
- ⬜ Docker support
- ⬜ Refresh token implementation

---

## 👨‍💻 Author

**Geovanny (Geowar17)**  
GitHub: [https://github.com/Geowar17](https://github.com/Geowar17)

---



