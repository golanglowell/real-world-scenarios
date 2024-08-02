# The URL Shortener

- Role: Web Services Beginner
- Task: Build a basic URL shortening service with an in-memory database

## Detailed Scenario:

Project Goal:
Create a simple web service that shortens long URLs into easily shareable short links.

### Main Features:

Accept long URLs via HTTP POST request
Generate unique short codes for each URL
Store URL mappings in memory
Redirect short URLs to their original long URLs


### Technical Requirements:

- Use the net/http package to create a web server
Implement two endpoints:
1. POST /shorten - to create short URLs
2. GET /{shortcode} - to redirect to the original URL
- Use a map[string]string to store short code -> long URL mappings
Generate random alphanumeric codes for short URLs


### Bonus Challenges:

- Add basic input validation (e.g., check if the input is a valid URL)
- Implement a simple cache expiration mechanism
- Create a basic HTML form for URL submission


### Learning Outcomes:

- Understanding HTTP handlers in Go
Working with maps for in-memory storage
- URL parsing and validation
- Generating random strings
- Basic error handling in a web context

### Discussion Points:

- How to ensure uniqueness of short codes
- Scalability considerations for larger systems
- Security implications of user-submitted URLs
- Potential for adding persistence (e.g., database storage)