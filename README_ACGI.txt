README.md

# ACGI 24×7 Support Portal

## Overview
ACGI 24×7 Support Portal is a centralized support management platform designed for ACG Inspections Pvt. Ltd. to manage customer service requests, support calls, issue tracking, team performance, SOP management, feedback collection, and operational analytics.

## Features
- User Registration, Login, OTP Verification
- Role-Based Access Control (RBAC)
- Call Logging and Resolution Tracking
- Open Call Monitoring
- Live Dashboard & Analytics
- Champion Dashboard
- Team Performance Monitoring
- SOP Repository
- Non-AMC Follow-up Tracking
- Repeated Issue Analytics
- Team Feedback Portal
- Audit Logs & Reporting

## Recommended Tech Stack
Frontend:
- HTML5
- CSS3
- JavaScript
- Chart.js
- XLSX.js

Backend:
- Node.js
- NestJS
- TypeScript

Database:
- PostgreSQL

Cache:
- Redis

Storage:
- Azure Blob Storage / AWS S3

Authentication:
- JWT + Refresh Tokens + OTP

## Architecture
Frontend -> API Gateway -> Services (Auth, Calls, SOPs, Feedback, Analytics) -> PostgreSQL + Redis + Blob Storage

## User Roles
- Service Engineer
- Service Region Team Lead
- QA Engineer
- QA Team Lead
- QA Manager / Head
- Service Manager / Head
- Operations Head
- Admin

## Core Modules
1. Authentication & User Management
2. Call Management
3. Dashboard & Analytics
4. Open Call Tracker
5. Champion Dashboard
6. Performance Dashboard
7. SOP Repository
8. Non-AMC Management
9. Repeated Issue Tracking
10. Team Feedback System
11. Audit Logs

## Key APIs
POST /auth/signup
POST /auth/login
POST /auth/send-otp
POST /auth/verify-otp

POST /calls
GET /calls
PUT /calls/:id
POST /calls/:id/close

GET /dashboard/summary
GET /analytics/status
GET /analytics/root-cause
GET /analytics/platform

GET /champions/week
GET /champions/month
GET /performance

POST /feedback
GET /feedback

POST /sops
GET /sops
DELETE /sops/:id

## Security
- JWT Authentication
- Bcrypt Password Hashing
- RBAC
- Audit Logging
- Input Validation
- API Rate Limiting

## Folder Structure
src/
├── auth/
├── users/
├── calls/
├── dashboard/
├── analytics/
├── champions/
├── performance/
├── feedback/
├── sops/
├── logs/
├── notifications/
├── database/
├── common/
└── main.ts

## Roadmap
Phase 1: Authentication & Users
Phase 2: Call Logging & Tracking
Phase 3: Dashboard & Analytics
Phase 4: Champions & Performance
Phase 5: SOP Repository
Phase 6: Feedback Module
Phase 7: Notifications & Integrations
Phase 8: Reporting & Audit Logs

## Author
ACG Inspections Pvt. Ltd.
Project: ACGI 24×7 Support Portal

## License
Private Internal Enterprise Application
Copyright © ACG Inspections Pvt. Ltd.
