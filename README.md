🧠1. SYSTEM ARCHITECTURE

Client (React / Postman)
        ↓
Backend API (Spring Boot / Node.js)
        ↓
Database (PostgreSQL)
        ↓
Cache (Redis)
        ↓
Queue (Kafka / RabbitMQ)

---------------------------------

⚙️ 2. TECH STACK

Backend: Java + Spring Boot
Database: PostgreSQL
Cache: Redis
Queue: Kafka (or RabbitMQ if simpler)
Deployment: Docker + AWS / Render

----------------------------------

📅 3. BUILD IN PHASES (Execution Plan)
🟢 Phase 1 – Core Backend (Week 1–2)

Focus: Make it WORK first

Features:
User Signup/Login (JWT Auth)
Event/Movie Listing API
Seat Layout (like A1, A2, B1…)
Booking API (simple, no concurrency handling yet)
Database Design (Important)

Tables:

users
events
shows
seats
bookings

👉 Key idea:

Each seat = one row (don’t store as JSON)