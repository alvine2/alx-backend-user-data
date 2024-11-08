# Simple API

A lightweight HTTP API to interact with the `User` model.

## File Structure

### `models/`

- `base.py`: Base class for all models in the API, managing file-based serialization.
- `user.py`: Defines the structure and attributes of the `User` model.

### `api/v1`

- `app.py`: Main entry point for the API.
- `views/index.py`: Defines foundational endpoints: `/status` and `/stats`.
- `views/users.py`: Includes all user-related API endpoints.

## Setup Instructions

To install dependencies:

```bash
pip3 install -r requirements.txt
```

## Running the API

Start the API with the following command:

```bash
API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
```

## API Endpoints

- **`GET /api/v1/status`**: Provides the current status of the API.
- **`GET /api/v1/stats`**: Returns statistical data about API usage.
- **`GET /api/v1/users`**: Lists all users in the system.
- **`GET /api/v1/users/:id`**: Retrieves a specific user by their ID.
- **`DELETE /api/v1/users/:id`**: Removes a user based on their ID.
- **`POST /api/v1/users`**: Creates a new user with required JSON fields `email` and `password`, and optional fields `last_name` and `first_name`.
- **`PUT /api/v1/users/:id`**: Updates a user’s details by ID with optional JSON fields `last_name` and `first_name`. 

This layout provides an easy way to manage and interact with user data while maintaining modularity and clarity in file organization.