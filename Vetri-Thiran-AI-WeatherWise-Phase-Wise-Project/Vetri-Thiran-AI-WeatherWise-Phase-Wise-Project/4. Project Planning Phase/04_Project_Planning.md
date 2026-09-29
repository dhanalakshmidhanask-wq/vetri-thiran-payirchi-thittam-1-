# Phase 4 – Project Planning Phase

## Development Timeline

| Week | Activity | Deliverable |
|---|---|---|
| 1 | Brainstorming | Problem and solution |
| 2 | Requirements | Functional/non-functional requirements |
| 3 | Design | Architecture and database |
| 4 | Authentication | Register/login/profile |
| 5 | Locations | Favorite-location CRUD |
| 6 | Weather | OpenWeatherMap integration |
| 7 | AI | Gemini summary and recommendation |
| 8 | Testing | Postman/API testing |
| 9 | Documentation | Technical documentation |
| 10 | Demonstration | Final project demo |

## Risks and Mitigation

| Risk | Mitigation |
|---|---|
| Weather API key unavailable | Deterministic mock fallback |
| Gemini API unavailable | Rule-based AI fallback |
| Unauthorized access | JWT middleware |
| Duplicate favorite city | Compound unique index |
| Database failure | Connection/error handling |
| Invalid user input | Controller validation |

## Completion Criteria
- Authentication APIs work
- Location CRUD works
- Weather endpoint works
- AI endpoints work
- Protected routes reject unauthenticated requests
- Postman collection can exercise the APIs
- Documentation and demonstration are complete
