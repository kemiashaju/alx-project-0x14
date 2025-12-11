# alx-project-0x14
API Overview

The Movie Database (TMDb) API gives developers programmatic access to a large and up‑to‑date collection of information about movies, TV shows, and people (actors, crew, etc.). You can search by title or name, discover new or trending content, retrieve detailed metadata (such as release dates, genre, overview, cast, crew, images, etc.), and access additional resources like images or credits. The API supports multiple languages and covers both film and television — making it ideal for building movie/TV‑centric applications, catalogs, recommendation engines, or streaming helper apps.

Version

The API version currently in use is v3. 
The Movie Database (TMDB)
+1

Available Endpoints

Here are some of the main endpoints available through TMDb:

/search/movie — Search for movies by title. Returns a list of movies matching the query. 
The Movie Database (TMDB)

/search/tv — Search for TV shows by name. (Analogous to movie search — not always separately documented, but part of the “search” category.)

/search/person — Search for people (actors, directors, etc.) by name.

/search/multi — Search across multiple categories (movies, TV shows, people) in a single request. 
The Movie Database (TMDB)
+1

/movie/{movie_id} — Get full details of a movie by its TMDb ID. Metadata includes title, overview, release date, genres, runtime, popularity, poster/backdrop paths, etc. 
The Movie Database (TMDB)
+2
Our World in Data
+2

/movie/{movie_id}/credits — Retrieve cast and crew information for a given movie (actors, directors, crew roles, etc.). 
PublicAPI
+1

/movie/{movie_id}/images — Get image resources associated with a movie (posters, backdrops, stills, etc.). 
PublicAPI
+1

/movie/popular — Get a list of currently popular movies (by popularity metric). 
The Movie Database (TMDB)
+1

/discover/movie — More advanced querying: discover movies based on filters (e.g. genre, release date, etc.). The “popular” endpoint is essentially a wrapper around a discover call with default filters. 
The Movie Database (TMDB)
+1

/configuration — Fetch static configuration data from TMDb, such as base URLs, valid image sizes, secure base URLs, and other needed configuration for building image URLs. 