# User Authentication Service

Build a user authentication service based on sessions

## Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/yourusername/user-authentication-service.git
    ```

2. **Navigate to the project directory**

    ```bash
    cd user-authentication-service
    ```

3. **Install dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Set environment variables**
    - `API_HOST` (e.g., `0.0.0.0`)
    - `API_PORT` (e.g., `5000`)
    - `SECRET_KEY` for session management

## Usage

1. **Start the Flask application**

    ```bash
    python3 app.py
    ```

2. **Interact with the API endpoints using tools like `curl` or Postman**

## API Endpoints

| Method | Endpoint            | Description                                                       |
|--------|---------------------|-------------------------------------------------------------------|
| GET    | `/`                 | Returns a welcome message                                        |
| POST   | `/users`            | Registers a new user                                             |
| POST   | `/sessions`         | Logs in a user and creates a session                             |
| DELETE | `/sessions`         | Logs out a user and destroys their session                       |
| GET    | `/profile`          | Retrieves the user's profile based on the session ID provided    |
