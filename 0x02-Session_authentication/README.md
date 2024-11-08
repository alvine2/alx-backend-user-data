# Simple API

A basic HTTP API for interacting with a `User` model.

## Directory Structure

### `models/`

- `base.py`: Contains the base model class for the API, managing serialization to file.
- `user.py`: Defines the `User` model.

### `api/v1/`

- `app.py`: Main entry point for the API.
- `views/index.py`: Contains basic endpoints like `/status` and `/stats`.
- `views/users.py`: Contains all user-related endpoints.

## Setup

Install the required packages:

```bash
$ pip3 install -r requirements.txt
```

## Running the API

To start the API, run:

```bash
$ API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
```

## Available Endpoints

- `GET /api/v1/status`: Returns the status of the API.
- `GET /api/v1/stats`: Provides statistics about the API.
- `GET /api/v1/users`: Lists all users.
- `GET /api/v1/users/:id`: Retrieves a user by ID.
- `DELETE /api/v1/users/:id`: Deletes a user by ID.
- `POST /api/v1/users`: Creates a new user (requires JSON fields `email`, `password`; optional `last_name` and `first_name`).
- `PUT /api/v1/users/:id`: Updates user information by ID (optional JSON fields `last_name` and `first_name`).