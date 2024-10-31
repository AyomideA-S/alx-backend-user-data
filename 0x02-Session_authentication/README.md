# Simple API

A simple HTTP API for managing `User` models.

## Files

### `models/`

- `base.py`: Handles serialization to file.
- `user.py`: Defines the User model.

### `api/v1`

- `app.py`: Entry point of the API.
- `views/index.py`: Endpoints: `/status`, `/stats`.
- `views/users.py`: User-related endpoints.

## Setup

```bash
pip3 install -r requirements.txt
```

## Run

```bash
API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
```

## Routes

- **GET** `/api/v1/status`: API status.
- **GET** `/api/v1/stats`: API statistics.
- **GET** `/api/v1/users`: List of users.
- **GET** `/api/v1/users/:id`: Get user by ID.
- **DELETE** `/api/v1/users/:id`: Delete user by ID.
- **POST** `/api/v1/users`: Create user (JSON: `email`, `password`, optional `last_name`, `first_name`).
- **PUT** `/api/v1/users/:id`: Update user by ID (JSON: `last_name`, `first_name`).
