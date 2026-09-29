# Phase 2 – Requirement Analysis

## Functional Requirements

| ID | Requirement | Description |
|---|---|---|
| FR-01 | Registration | Create a user account |
| FR-02 | Login | Authenticate and return JWT |
| FR-03 | Profile | Retrieve authenticated user profile |
| FR-04 | Add Location | Save a favorite city and country |
| FR-05 | List Locations | View the user's favorite locations |
| FR-06 | Update Location | Edit a saved location |
| FR-07 | Delete Location | Remove a saved location |
| FR-08 | Weather | Fetch current weather for a city |
| FR-09 | AI Summary | Generate a natural-language weather summary |
| FR-10 | AI Recommendation | Generate practical weather recommendations |

## Non-Functional Requirements
- Secure password hashing
- JWT-protected private APIs
- RESTful API design
- MongoDB persistence
- Graceful fallback when external API keys are missing or fail
- Modular controllers, routes, services and models

## Environment Variables
```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/weatherwise
JWT_SECRET=your_super_secret_jwt_key
OPENWEATHER_API_KEY=your_openweathermap_api_key
GEMINI_API_KEY=your_gemini_api_key
```

## API Groups
- `/api/auth`
- `/api/locations`
- `/api/weather`
- `/api/ai`
