# Phase 5 – Project Development Phase

## Technology Stack
- Node.js 18+
- Express.js
- MongoDB
- Mongoose
- Google Gemini API
- OpenWeatherMap API
- JWT
- bcryptjs
- CORS
- dotenv
- Nodemon

## Project Structure

```text
Backend/
├── package.json
├── package-lock.json
├── README.md
├── postman_collection.json
└── src/
    ├── server.js
    ├── app.js
    ├── config/
    │   └── db.js
    ├── models/
    │   ├── User.js
    │   └── Location.js
    ├── middleware/
    │   └── authMiddleware.js
    ├── controllers/
    │   ├── authController.js
    │   ├── locationController.js
    │   ├── weatherController.js
    │   └── aiController.js
    ├── routes/
    │   ├── authRoutes.js
    │   ├── locationRoutes.js
    │   ├── weatherRoutes.js
    │   └── aiRoutes.js
    └── services/
        ├── weatherService.js
        └── aiService.js
```

## Development Flow

1. Configure Node.js and dependencies.
2. Connect MongoDB.
3. Implement user model and authentication.
4. Add JWT protection.
5. Implement favorite-location CRUD.
6. Integrate OpenWeatherMap.
7. Integrate Gemini AI.
8. Add fallback logic.
9. Test all endpoints with Postman.

## Run Commands

```bash
npm install
npm run dev
```

Production:
```bash
npm start
```

Server:
```text
http://localhost:5000
```

## Main Endpoints

### Auth
- POST `/api/auth/register`
- POST `/api/auth/login`
- GET `/api/auth/profile`

### Locations
- POST `/api/locations`
- GET `/api/locations`
- PUT `/api/locations/:id`
- DELETE `/api/locations/:id`

### Weather
- GET `/api/weather/:city`

### AI
- POST `/api/ai/weather-summary`
- POST `/api/ai/weather-recommendation`
