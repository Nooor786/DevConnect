# Deployment outline
Vercel: frontend root `client`, build `npm run build`, output `dist`.
Railway: backend workspace, build `npm run build`, start `npm run start`.
Neon: PostgreSQL; set DATABASE_URL and run `npx prisma migrate deploy`.
Set CLIENT_URL, JWT_SECRET, COOKIE_SECURE=true and HTTPS. Free tier limits may change.
