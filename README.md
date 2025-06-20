# 🎬 MoviesDatabase API Integration

This project integrates with the [MoviesDatabase API](https://rapidapi.com/SAdrian/api/moviesdatabase) to retrieve movie, TV show, and actor data. It demonstrates how to consume a third-party REST API using HTTP requests and handle data responses efficiently.

---

## 📖 API Overview

The MoviesDatabase API provides access to a large catalog of movies, TV series, actors, and crew information. It supports searching by title, actor, or ID, and returns detailed metadata including release dates, genres, posters, and plot summaries.

### Key Features:
- Search movies and TV shows by title or IMDb ID
- Get detailed information for titles and people
- Retrieve lists such as "Most Popular" or "Trending"
- Access images, descriptions, and related metadata

---

## 📌 Version

**API Version:** `1.0.0`  
(As listed on RapidAPI)

---

## 📂 Available Endpoints

| Endpoint | Description |
|----------|-------------|
| `/titles/search/title/{title}` | Search for movies or TV shows by title. |
| `/titles/x/titles-by-ids` | Get detailed data on multiple titles using IMDb IDs. |
| `/actors/{actor_id}` | Get details about an actor using their ID. |
| `/titles/{title_id}` | Fetch complete information about a movie or show. |
| `/titles/utils/genres` | Retrieve a list of all available genres. |
| `/titles/random` | Get a random movie or show recommendation. |

---

## 🔄 Request and Response Format

### Example Request (Search by Title):

```http
GET https://moviesdatabase.p.rapidapi.com/titles/search/title/Inception
Headers:
  X-RapidAPI-Key: YOUR_API_KEY
  X-RapidAPI-Host: moviesdatabase.p.rapidapi.com
