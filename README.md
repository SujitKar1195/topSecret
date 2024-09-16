<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
</head>
<body>

<div class="container">
    <h1>Project Name: topSecret</h1>
    <p>A simple web application for user registration, login, and storing secrets. Includes authentication using Passport.js (Local and Google OAuth 2.0 strategies) and PostgreSQL for data storage.</p>

    <div class="section">
        <h2>Table of Contents</h2>
        <ul>
            <li><a href="#features">Features</a></li>
            <li><a href="#installation">Installation</a></li>
            <li><a href="#usage">Usage</a></li>
            <li><a href="#endpoints">Endpoints</a></li>
            <li><a href="#technologies">Technologies Used</a></li>
            <li><a href="#contributing">Contributing</a></li>
            <li><a href="#license">License</a></li>
        </ul>
    </div>

    <div id="features" class="section">
        <h2>Features</h2>
        <ul>
            <li>User Registration and Login using Passport.js</li>
            <li>Google OAuth 2.0 for social login</li>
            <li>Storing and retrieving user secrets</li>
            <li>Session management using <code>express-session</code></li>
            <li>PostgreSQL as the database for user data</li>
        </ul>
    </div>

    <div id="installation" class="section">
        <h2>Installation</h2>
        <p>Follow these steps to set up the project locally:</p>
        <ol>
            <li>Clone the repository:</li>
            <pre><code>git clone https://github.com/yourusername/your-repo-name.git</code></pre>
            <li>Navigate to the project directory:</li>
            <pre><code>cd your-repo-name</code></pre>
            <li>Install dependencies:</li>
            <pre><code>npm install</code></pre>
            <li>Create a <code>.env</code> file and add the following variables:</li>
            <div class="highlight">
                PG_USER=your_pg_user<br>
                PG_HOST=your_pg_host<br>
                PG_DATABASE=your_pg_database<br>
                PG_PASSWORD=your_pg_password<br>
                PG_PORT=your_pg_port<br>
                SESSION_SECRET=your_session_secret<br>
                GOOGLE_CLIENT_ID=your_google_client_id<br>
                GOOGLE_CLIENT_SECRET=your_google_client_secret<br>
            </div>
            <li>Start the application:</li>
            <pre><code>npm start</code></pre>
        </ol>
    </div>

    <div id="usage" class="section">
        <h2>Usage</h2>
        <p>After starting the application, you can access the following endpoints:</p>
        <ul>
            <li>Home: <code>http://localhost:3000/</code></li>
            <li>Login: <code>http://localhost:3000/login</code></li>
            <li>Register: <code>http://localhost:3000/register</code></li>
            <li>Secrets: <code>http://localhost:3000/secrets</code> (Requires authentication)</li>
        </ul>
    </div>

    <div id="endpoints" class="section">
        <h2>Endpoints</h2>
        <ul>
            <li><code>GET /</code> - Render the home page</li>
            <li><code>GET /login</code> - Render the login page</li>
            <li><code>GET /register</code> - Render the registration page</li>
            <li><code>POST /login</code> - Authenticate user using local strategy</li>
            <li><code>POST /register</code> - Register a new user</li>
            <li><code>GET /auth/google</code> - Initiate Google OAuth 2.0 login</li>
            <li><code>POST /submit</code> - Submit a secret (Authenticated users only)</li>
        </ul>
    </div>

    <div id="technologies" class="section">
        <h2>Technologies Used</h2>
        <ul>
            <li>Node.js</li>
            <li>Express</li>
            <li>Passport.js (Local and Google OAuth 2.0 strategies)</li>
            <li>PostgreSQL</li>
            <li>Bcrypt for password hashing</li>
            <li>EJS for templating</li>
        </ul>
    </div>

    <div id="contributing" class="section">
        <h2>Contributing</h2>
        <p>Contributions are welcome! Please follow these steps:</p>
        <ol>
            <li>Fork the repository</li>
            <li>Create a new branch (<code>git checkout -b feature-branch</code>)</li>
            <li>Commit your changes (<code>git commit -m 'Add new feature'</code>)</li>
            <li>Push to the branch (<code>git push origin feature-branch</code>)</li>
            <li>Create a new Pull Request</li>
        </ol>
    </div>

    <div id="license" class="section">
        <h2>License</h2>
        <p>This project is licensed under the MIT License.</p>
    </div>
</div>

</body>
</html>
