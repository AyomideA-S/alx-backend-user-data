# Simple API

A simple HTTP API for managing `User` models.

## Files

### `models/`

- **base.py**: Handles model serialization to file.
- **user.py**: Defines the User model.

### `api/v1`

- **app.py**: Entry point of the API.
- **views/index.py**: Basic endpoints: `/status` and `/stats`.
- **views/users.py**: User-related endpoints.

## Setup

```bash
pip3 install -r requirements.txt
```

## Run

```bash
API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
```

## Routes

| Method | Endpoint            | Description                                                     |
|--------|---------------------|-----------------------------------------------------------------|
| GET    | `/api/v1/status`    | Returns the status of the API                                   |
| GET    | `/api/v1/stats`     | Returns API statistics                                           |
| GET    | `/api/v1/users`     | Returns the list of users                                        |
| GET    | `/api/v1/users/:id` | Returns a user based on the ID                                  |
| DELETE | `/api/v1/users/:id` | Deletes a user based on the ID                                  |
| POST   | `/api/v1/users`     | Creates a new user (Parameters: `email`, `password`, `last_name` (optional), `first_name` (optional)) |
| PUT    | `/api/v1/users/:id` | Updates a user based on the ID (Parameters: `last_name`, `first_name`) |
