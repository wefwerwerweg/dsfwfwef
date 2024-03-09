# Anime API

An API for an anime streaming site built with Django REST Framework.

## API Routes

### Authentication
- **POST /api/register**: Create a new user account.
- **POST /api/login**: Log in with user credentials.
- **POST /api/logout**: Log out the authenticated user.
- **POST /api/change-password**: Change the password for the authenticated user.

### User Profile
- **GET /api/user/profile**: Get the profile information of the authenticated user.
- **GET /api/user/detail/{user_id}**: Get the profile information of a specific user.
- **DELETE /api/user/delete**: Delete the authenticated user account.

### Anime
- **GET /api/anime/list**: Get a list of all anime.
- **GET /api/anime/{pk}**: Get detailed information about a specific anime.
- **POST /api/anime/create**: Create a new anime entry.
- **PUT /api/anime/update/{anime_id}**: Update an existing anime entry.
- **DELETE /api/anime/delete/{anime_id}**: Delete a specific anime entry.

### Favorites
- **POST /api/favorites/add/{anime_id}**: Add an anime to the user's favorites.
- **POST /api/favorites/remove/{anime_id}**: Remove an anime from the user's favorites.
- **GET /api/favorites/list**: Get a list of the user's favorite anime.

### Anime Sorting and Filtering
- **GET /api/anime/filter/{parameters}**: Get a list of anime filtered by specific parameters (e.g., genre, year, status).

### Search
- **GET /api/anime/search?query={search_query}**: Search for anime based on a given query.

### Miscellaneous
- **GET /api/anime/random**: Get a random anime.
- **GET /api/anime/continue-watching**: Get the list of anime the user is currently watching.
- **GET /api/anime/most-popular**: Get a list of the most popular anime.
- **GET /api/anime/most-famous**: Get a list of the most famous anime.
- **GET /api/anime/recently-added**: Get a list of recently added anime series.
- **GET /api/anime/movies**: Get a list of anime movies.
- **GET /api/anime/history**: Get the user's anime view history.
- **GET /api/anime/watched**: Get the list of anime the user has watched.

### Anime Episodes
- **GET /api/anime/{anime_id}/episodes**: Get a list of episodes for a specific anime.
- **GET /api/anime/{anime_id}/episodes/{episode_id}**: Get detailed information about a specific episode.
- **POST /api/anime/{anime_id}/episodes/create**: Create a new episode for an anime.
- **PUT /api/anime/{anime_id}/episodes/update/{episode_id}**: Update an existing episode.
- **DELETE /api/anime/{anime_id}/episodes/delete/{episode_id}**: Delete a specific episode.

### Reviews and Ratings
- **POST /api/anime/{anime_id}/reviews/create**: Create a review for an anime.
- **PUT /api/anime/{anime_id}/reviews/update/{review_id}**: Update an existing review.
- **DELETE /api/anime/{anime_id}/reviews/delete/{review_id}**: Delete a specific review.
- **POST /api/anime/{anime_id}/ratings/rate**: Rate an anime.
- **PUT /api/anime/{anime_id}/ratings/update**: Update a rating for an anime.

### Recommendations
- **GET /api/anime/{anime_id}/recommendations**: Get a list of recommended anime based on a specific anime.

### Categories and Tags
- **GET /api/categories**: Get a list of anime categories.
- **GET /api/categories/{category_id}/anime**: Get a list of anime in a specific category.
- **GET /api/tags**: Get a list of anime tags.
- **GET /api/tags/{tag_id}/anime**: Get a list of anime associated with a specific tag.

### User Interactions
- **POST /api/anime/{anime_id}/like**: Like an anime.
- **POST /api/anime/{anime_id}/dislike**: Dislike an anime.
- **POST /api/anime/{anime_id}/comments/create**: Create a comment for an anime.
- **PUT /api/anime/{anime_id}/comments/update/{comment_id}**: Update an existing comment.
- **DELETE /api/anime/{anime_id}/comments/delete/{comment_id}**: DeleteI apologize for the incomplete response. Here's the continuation of the API routes in markdown format:

### User Interactions
- **POST /api/anime/{anime_id}/like**: Like an anime.
- **POST /api/anime/{anime_id}/dislike**: Dislike an anime.
- **POST /api/anime/{anime_id}/comments/create**: Create a comment for an anime.
- **PUT /api/anime/{anime_id}/comments/update/{comment_id}**: Update an existing comment.
- **DELETE /api/anime/{anime_id}/comments/delete/{comment_id}**: Delete a specific comment.

### Subscription and Notifications
- **POST /api/subscription/subscribe**: Subscribe to receive notifications for new anime releases or updates.
- **POST /api/subscription/unsubscribe**: Unsubscribe from receiving notifications.
