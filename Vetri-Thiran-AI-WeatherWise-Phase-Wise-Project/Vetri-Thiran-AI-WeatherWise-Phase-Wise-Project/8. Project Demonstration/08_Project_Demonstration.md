# Phase 8 – Project Demonstration

## Demo Sequence

### Step 1 – Start the Backend
```bash
npm install
npm run dev
```

### Step 2 – Register
```text
POST /api/auth/register
```

Example:
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "123456"
}
```

### Step 3 – Login
```text
POST /api/auth/login
```
Save the returned JWT token.

### Step 4 – View Profile
```text
GET /api/auth/profile
```
Use Bearer token authentication.

### Step 5 – Add Favorite City
```text
POST /api/locations
```

```json
{
  "city": "Chennai",
  "country": "India"
}
```

### Step 6 – View Favorites
```text
GET /api/locations
```

### Step 7 – Fetch Weather
```text
GET /api/weather/Chennai
```

### Step 8 – Generate AI Summary
```text
POST /api/ai/weather-summary
```

```json
{
  "city": "Chennai",
  "temperature": 31,
  "humidity": 70,
  "condition": "Sunny"
}
```

### Step 9 – Generate AI Recommendation
```text
POST /api/ai/weather-recommendation
```

```json
{
  "temperature": 31,
  "condition": "Sunny"
}
```

### Step 10 – Demonstrate Fallback
Temporarily omit API keys and show that the backend can return mock/rule-based responses.

## Presentation Order
1. Problem
2. Proposed solution
3. Objectives
4. Architecture
5. Technology stack
6. Database models
7. Authentication
8. Weather API
9. Gemini AI
10. Testing
11. Future enhancements
