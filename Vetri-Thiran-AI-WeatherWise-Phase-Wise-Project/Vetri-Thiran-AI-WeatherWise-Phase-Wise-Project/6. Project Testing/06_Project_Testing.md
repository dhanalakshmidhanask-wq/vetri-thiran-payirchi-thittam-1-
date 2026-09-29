# Phase 6 – Project Testing

## Testing Method
The API is tested using the supplied Postman collection.

## Test Cases

| ID | Test | Expected Result |
|---|---|---|
| TC-01 | Register valid user | Account and JWT returned |
| TC-02 | Register duplicate email | Validation/error response |
| TC-03 | Login valid user | JWT returned |
| TC-04 | Login invalid password | Authentication error |
| TC-05 | Profile without token | 401 response |
| TC-06 | Profile with valid token | User profile returned |
| TC-07 | Add favorite location | Location created |
| TC-08 | Get favorites | User locations returned |
| TC-09 | Update favorite | Location updated |
| TC-10 | Delete favorite | Location removed |
| TC-11 | Weather by city | Weather metrics returned |
| TC-12 | AI summary with valid data | Summary returned |
| TC-13 | AI recommendation | Recommendation returned |
| TC-14 | AI endpoint without token | 401 response |
| TC-15 | Missing required fields | 400 response |
| TC-16 | Missing external API key | Mock/fallback response |

## AI Testing
Test both:
- Gemini API configured
- Gemini API not configured

The application is designed to continue with local rule-based responses when Gemini is unavailable.

## Weather Testing
Test:
- Valid city
- Unknown city
- Missing OpenWeatherMap key
- Invalid API key
