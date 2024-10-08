
# Project Name: topSecret

A simple web application for user registration, login, and storing secrets. Includes authentication using Passport.js (Local and Google OAuth 2.0 strategies) and PostgreSQL for data storage.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)


## Features

- User Registration and Login using Passport.js
- `Google OAuth 2.0` for social login
- Storing and retrieving user secrets
- Session management using `express-session`
- `PostgreSQL` as the database for user data

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:

    ```bash
    git clone https://github.com/SujitKar1195/topSecret.git
    ```

2. Navigate to the project directory:

    ```bash
    cd your-repo-name
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Create a `.env` file and add the following variables:

    ```
    PG_USER=your_pg_user
    PG_HOST=your_pg_host
    PG_DATABASE=your_pg_database
    PG_PASSWORD=your_pg_password
    PG_PORT=your_pg_port
    SESSION_SECRET=your_session_secret
    GOOGLE_CLIENT_ID=your_google_client_id
    GOOGLE_CLIENT_SECRET=your_google_client_secret
    ```

5. Start the application:

    ```bash
    npm start
    ```

## Usage

After starting the application, you can access the following endpoints:

- Home: `http://localhost:3000/`
- Login: `http://localhost:3000/login`
- Register: `http://localhost:3000/register`
- Secrets: `http://localhost:3000/secrets` (Requires authentication)

## Endpoints

- `GET /` - Render the home page
- `GET /login` - Render the login page
- `GET /register` - Render the registration page
- `POST /login` - Authenticate user using local strategy
- `POST /register` - Register a new user
- `GET /auth/google` - Initiate Google OAuth 2.0 login
- `POST /submit` - Submit a secret (Authenticated users only)

## Technologies Used

- Node.js
- Express
- Passport.js (Local and Google OAuth 2.0 strategies)
- PostgreSQL
- Bcrypt for password hashing
- EJS for templating

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new Pull Request


