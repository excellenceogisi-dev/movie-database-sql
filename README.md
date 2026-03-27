# Movie Database SQL Project

## Overview
This project is a **relational database for movies**, designed to store and manage information about films, actors, directors, genres, and user ratings. It demonstrates the use of **SQL concepts** including tables, relationships, constraints, queries, and data analysis.  

The database is ideal for **learning SQL**, building **data-driven applications**, or serving as a backend for a movie-related web or mobile application.

---

## Features
- **Movies table:** stores title, release year, genre, duration, and rating.  
- **Actors table:** stores actor details and their filmography.  
- **Directors table:** stores director details.  
- **Genres table:** stores movie genres.  
- **Ratings table:** stores user ratings for movies.  
- **SQL Queries included:**  
  - Select top-rated movies  
  - Find movies by a specific actor or director  
  - Count movies per genre  
  - Join tables to show actor-director collaborations  

---

## Database Schema

### Tables and Relationships
- `Movies` (MovieID, Title, ReleaseYear, GenreID, DirectorID, Duration, Rating)  
- `Actors` (ActorID, Name, BirthYear, Nationality)  
- `Directors` (DirectorID, Name, BirthYear, Nationality)  
- `Genres` (GenreID, Name)  
- `MovieActors` (MovieID, ActorID) – many-to-many relationship  
- `Ratings` (RatingID, MovieID, UserID, Score, Review)  

**Relationships:**  
- `Movies` → `Genres`: Many-to-One  
- `Movies` → `Directors`: Many-to-One  
- `Movies` ↔ `Actors`: Many-to-Many via `MovieActors`  
- `Movies` → `Ratings`: One-to-Many  

---

## Setup Instructions

1. Clone the repository:  
```bash
git clone https://github.com/yourusername/movie-database-sql.git
