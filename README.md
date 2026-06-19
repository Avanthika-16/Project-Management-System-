## 🚀 ProjectFlow – Project Management System
A modern app to help teams and individuals organize projects and tasks quickly and easily.

### 🔧 Tech Stack
- **Frontend:** React, Vite, Tailwind CSS, React Router  
- **Backend:** Node.js, Express.js, JWT, bcrypt  
- **Database:** MySQL with Sequelize ORM  
- **Extras:** Charts (Recharts), Forms (React Hook Form), API Docs (Swagger), Docker for deployment  

### ✨ Features
- **Authentication:** Register, login, logout with secure JWT tokens  
- **Projects:** Create, view, edit, delete projects with status tracking  
- **Tasks:** Full CRUD with priority levels and status updates  
- **Dashboard:** Real-time stats, charts, and recent activity  
- **Search & Filter:** Find projects/tasks by name, status, or priority  
- **Pagination:** Server-side pagination for large datasets  
- **Responsive:** Works on desktop, tablet, and mobile  
- **Secure:** Password hashing, rate limiting, input validation  

### 📂 Project Structure
```
ProjectFlow/
├── client/   # React frontend
│   ├── src/
│   │   ├── api/        # API services
│   │   ├── components/ # UI components
│   │   ├── context/    # Auth, Toast
│   │   ├── hooks/      # Custom hooks
│   │   ├── pages/      # Page components
│   │   ├── routes/     # Router config
│   │   └── utils/      # Helpers
├── server/   # Express backend
│   ├── config/      # DB config
│   ├── controllers/ # Route handlers
│   ├── middleware/  # Auth, validation
│   ├── models/      # Sequelize models
│   ├── routes/      # API routes
│   ├── validators/  # Input rules
│   ├── swagger/     # API docs
├── docker-compose.yml
└── README.md
```

### ⚙️ Getting Started
**Option 1: Docker (easy way)**  
1. Clone repo  
2. Run `docker-compose up --build`  
3. Access:  
   - Frontend → `http://localhost:3000`  
   - Backend → `http://localhost:5000`  
   - API Docs → `http://localhost:5000/api-docs`  

**Option 2: Run locally**  
- Create MySQL database: `CREATE DATABASE projectflow;`  
- Backend: `cd server && npm install && cp .env.example .env && npm run dev`  
- Frontend: `cd client && npm install && cp .env.example .env && npm run dev`  

### 🔑 Environment Variables
**Backend (.env):**
```
PORT=5000
DB_HOST=localhost
DB_PORT=3306
DB_NAME=projectflow
DB_USER=root
DB_PASSWORD=your_password
JWT_SECRET=your-secret
CLIENT_URL=http://localhost:5173
```

**Frontend (.env):**
```
VITE_API_URL=http://localhost:5000/api
```

### 📡 API Endpoints
- **Auth:** `/api/auth/register`, `/api/auth/login`, `/api/auth/logout`, `/api/auth/me`  
- **Projects:** `/api/projects` (CRUD)  
- **Tasks:** `/api/tasks` (CRUD, filters, pagination)  
- **Dashboard:** `/api/dashboard/stats`  

### 🗄 Database Schema
- **User → Projects → Tasks**  
- One user can have many projects, and each project can have many tasks.  
- Cascade delete ensures linked data is cleaned up automatically.  

### 📖 License
MIT — free to use, modify, and share.  
