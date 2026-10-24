
# SENG3080 Week 7 Backend Lab

## Description
A database-backed Express Task API using Sequelize,
SQLite, Passport authentication, input validation,
security middleware, and Redis caching.

## Installation
npm install

## Environment Configuration
Create a .env file containing:

PORT=3000
SESSION_SECRET=your-session-secret
REDIS_URL=redis://localhost:6379

## Start Redis
docker run -d --name week7-redis -p 6379:6379 redis:7-alpine

For an existing container:
docker start week7-redis

## Run Application
npm run dev

## API Endpoints
GET /api/tasks
GET /api/tasks/:id
POST /api/tasks
PUT /api/tasks/:id
DELETE /api/tasks/:id

POST /api/auth/register
POST /api/auth/login
GET /api/auth/me

## Testing
Use Postman to test routing, CRUD operations,
validation, authentication, security headers,
and Redis caching.
