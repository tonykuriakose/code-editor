# 🚀 Microservices-Based Code Collaboration Platform

## 📂 Project Structure
```
backend/                        # Root backend directory
├── api-gateway/                # API Gateway (Express, JWT, Authentication)
├── services/                   # Microservices
│   ├── user-service/           # User management (Auth, Profile)
│   ├── code-execution-service/ # Code execution (Docker, Sandboxing)
│   ├── collaboration-service/  # Real-time editing (Socket.io, WebRTC)
│   ├── file-storage-service/   # Save/load user files (MongoDB, Redis)
├── shared/                     # Shared utilities (Logging, DB, Configs)
├── Dockerfile                  # Docker configuration
├── package.json                # Dependencies & scripts
├── tsconfig.json               # TypeScript configuration
├── .env                        # Environment variables
└── README.md                   # Project documentation
```

## 🏗️ Clean Architecture
Each microservice follows Clean Architecture principles:
```
service-name/
├── src/
│   ├── application/         # Use cases (business logic)
│   ├── domain/              # Entities (core business models)
│   ├── infrastructure/      # External integrations (DB, Redis, WebRTC, etc.)
│   ├── interfaces/          # Controllers, routes, event listeners
│   ├── shared/              # Common utilities and configurations
│   ├── index.ts             # Entry point
├── package.json
├── tsconfig.json
├── Dockerfile
└── README.md
```

## ⚙️ Tech Stack
- **Backend:** Node.js, Express, TypeScript
- **Authentication:** JWT, OAuth
- **Database:** MongoDB, Redis
- **Real-Time Collaboration:** Socket.io, WebRTC
- **Code Execution:** Docker-based sandboxing
- **API Gateway:** Express with authentication middleware

