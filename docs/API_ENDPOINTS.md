# API endpoints
All responses: `{success,data,message}`.
POST /api/auth/register, /api/auth/login, /api/auth/logout; GET /api/auth/me
GET/PUT /api/profile/me
GET/POST /api/projects; PUT/DELETE /api/projects/:id
GET/POST /api/posts
GET /api/users/search?q=&skill=&location=
POST /api/connections/:userId; PATCH/DELETE /api/connections/:id
POST /api/endorsements/:userId
GET /api/notifications
