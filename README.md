# alx-project-0x14
CineSeek is a sleek movie discovery app built with Next.js, TypeScript, and Tailwind CSS. It lets users explore and search for movies by genre or release year using the MoviesDatabase API, offering a fast, responsive, and type-safe experience.


## API Overview
The MoviesDatabase API is a powerful and comprehensive resource for film and television metadata. It offers detailed information on over 9 million titles—including movies, series, and episodes—and more than 11 million actors, crew, and cast members.
### Key features include:

- Movie and TV show details (titles, genres, release dates, etc.)
- Actor and crew profiles with full biographies
- Awards and nominations
- YouTube trailer links
- Search functionality by title, genre, or year

## The MoviesDatabase version used for this project is v1 (current)


## Available Endpoints
- **GET `/titles`**  
  Returns a list of titles (movies, series, episodes) with optional filters such as genre, year, and pagination.

- **GET `/titles/:id`**  
  Fetches detailed information about a specific title using its unique ID.

- **GET `/titles/search/title/:name`**  
  Allows searching for titles by name (partial or full match).

- **GET `/actors/:id`**  
  Provides detailed information about a specific actor including biography and filmography.

- **GET `/genres`**  
  Lists all available genres in the database.

- **GET `/years`**  
  Lists all years for which titles exist in the database.


## Request and Response Format
Requests use standard HTTP methods (mostly `GET`). Query parameters like title, year, or genre are passed in the URL.

## Authentication
X-RapidAPI-Key: YOUR_API_KEY  
X-RapidAPI-Host: moviesdatabase.p.rapidapi.com


 ## Error Handling
Common error codes:
-401 – Invalid or missing API key
-404 – Not found
-429 – Rate limit exceeded
-500 – Server error


## Usage Limits and Best Practices
 -Free plan has request limits.
 -Cache responses where possible.
 -Avoid sending too many requests in a short time.
 -Handle errors gracefully in the UI.
