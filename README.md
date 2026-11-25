# DevConnect — Developer Networking & Portfolio Platform
Code A Nova internship starter | React + Vite + TypeScript | Express + TypeScript | PostgreSQL + Prisma

## Setup
Install Node.js 20+ and PostgreSQL. Open this folder in VS Code.

Server terminal:
```powershell
cd server
Copy-Item .env.example .env
npm install
```
Edit `server/.env`: set DATABASE_URL and a long JWT_SECRET.
```powershell
npx prisma generate
npx prisma migrate dev --name init
npm run dev
```
Client terminal:
```powershell
cd client
Copy-Item .env.example .env
npm install
npm run dev
```
Open http://localhost:5173. API health: http://localhost:5000/health

## Included
Monorepo, Prisma schema, local registration/login, JWT httpOnly cookie, profile and skills, projects, technical blog, developer search, connection requests, skill endorsements, notifications persistence, Socket.io event channel, basic React UI, deployment/security documentation.

## Important scope notes
This is an educational starter, not a production-ready social network. GitHub OAuth and Cloudinary upload are not fully implemented in this starter; add them before claiming those requirements are complete. The starter includes avatar URL support. Complete all items in docs/15_DAY_PLAN.md and docs/SECURITY_CHECKLIST.md, test workflows, and add your own screenshots/results.

## Deployment
Frontend: Vercel (root client, build `npm run build`, output dist).
Backend: Railway (server workspace, build `npm run build`, start `npm run start`).
Database: Neon PostgreSQL. Configure production env vars and run `npx prisma migrate deploy`. Use HTTPS and secure cookies. Free-tier limits can change.
