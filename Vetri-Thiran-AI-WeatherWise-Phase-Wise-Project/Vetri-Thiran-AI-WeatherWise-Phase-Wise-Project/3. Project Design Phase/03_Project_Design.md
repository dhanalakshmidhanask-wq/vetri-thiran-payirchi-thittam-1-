# Phase 3 – Project Design Phase

## Architecture

```text
Client / Postman
       |
       v
   Express API
       |
       +--------------------+
       |                    |
   Auth Middleware       Routes
       |                    |
       +-----------> Controllers
                         |
              +----------+----------+
              |          |          |
           MongoDB    Weather     Gemini
           Mongoose   Service      AI Service
```

## Modules

### Authentication
Registration, login, password verification and JWT generation.

### Authorization
JWT middleware protects profile, location and AI routes.

### Location Management
Stores favorite city/country pairs associated with the authenticated user.

### Weather Service
Calls OpenWeatherMap and provides deterministic mock weather when an API key is not configured.

### AI Service
Uses Gemini 2.5 Flash for weather summaries and recommendations, with rule-based fallbacks.

## Database Design

### User
- name
- email
- password
- createdAt
- updatedAt

### Location
- city
- country
- user
- createdAt
- updatedAt

A unique compound index prevents the same user from saving the exact same city/country combination twice.

## Security
- bcryptjs password hashing
- JWT authentication
- Protected AI and location endpoints
- User-specific location access
