# Core Security API Features

## Project Overview
Core Security API Features is a hands-on backend project focused on building and understanding security-oriented API patterns. The project is implemented as a TypeScript + Express service that demonstrates core authentication workflows using Firebase Authentication and the Firebase Admin SDK.

The goal is to explore practical backend security concepts in a small, testable application, including request validation, token generation, token verification, and secure user handling. It serves as both a learning project and a foundation for expanding into more advanced security features such as role-based access control, rate limiting, and audit logging.

## Features
- Modular Express API structure with route-based organization
- Request validation using Zod schemas before processing user input
- Firebase Admin setup for secure server-side authentication flows
- Custom token generation for Firebase-based user authentication
- ID token verification through protected API endpoints
- Middleware-driven validation and centralized error handling
- Local development support with Firebase Emulator Suite concepts

## Technologies
- TypeScript for strong typing and safer backend development
- Node.js with Express for building the API server
- Firebase Admin SDK for server-side authentication and user management
- Firebase Authentication for token-based identity workflows
- Zod for schema validation and input enforcement
- dotenv for environment-based configuration
- ts-node-dev and nodemon for fast local development

## Lessons Learned
- Input validation is one of the first and most important security controls in any API.
- Authentication logic should be centralized and easy to test so that token handling remains consistent.
- Server-side verification of identity tokens is essential for protecting backend resources.
- Clear middleware and structured error responses improve both security and maintainability.
- Using local emulators makes it easier to experiment with authentication flows without risking production data.

## Getting Started
1. Install dependencies:
   ```bash
   cd core-security-api
   npm install
   ```
2. Start the development server:
   ```bash
   npm run dev
   ```
3. Explore the main API endpoints:
   - POST /api/users/create-custom-token
   - POST /api/users/verify-user-token

## Project Structure
- src/server.ts - entry point for the Express application
- src/routes/ - API route definitions
- src/middleware/ - reusable request validation middleware
- src/firebase/ - Firebase authentication helpers and admin initialization
- src/utils/ - schemas and shared types
