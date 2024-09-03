<h1>Backend Development Task - Orinson Technologies</h1>

<h2>Project Overview</h2>
<p>This project is a backend service for user authentication, including registration and login functionality. The backend is built using the following technologies:</p>
<ul>
    <li><strong>Express</strong> - A web framework for Node.js used to create the server and manage routing.</li>
    <li><strong>Mongoose</strong> - An ODM (Object Data Modeling) library for MongoDB and Node.js, used for database interaction.</li>
    <li><strong>MongoDB</strong> - A NoSQL database used to store user data.</li>
    <li><strong>Joi</strong> - A validation library used to validate user input on registration and login.</li>
    <li><strong>argon2</strong> - A password hashing algorithm used to securely hash user passwords.</li>
    <li><strong>nodemon</strong> - A tool that automatically restarts the server when file changes in the directory are detected, improving development workflow.</li>
</ul>

<h2>Setup Instructions</h2>
<ol>
    <li>Clone the repository to your local machine:
        <pre><code>git clone https://github.com/BereketZz/Orinson-Tech-task1.git</code></pre>
    </li>
    
  <li>Install the required dependencies:
        <pre><code>npm install</code></pre>
    </li>
    <li>Create a `.env` file in the root directory and add your MongoDB connection string:
        <pre><code>MONGO_URI=your_mongodb_connection_string</code></pre>
    </li>
    <li>Start the development server with nodemon:
        <pre><code>npm start</code></pre>
    </li>
</ol>

<h2>API Endpoints</h2>
<p>The following API endpoints are available:</p>
<ul>
    <li><code>POST /auth/register</code> - Register a new user with an email and password. The password is hashed using argon2.</li>
    <li><code>POST /auth/login</code> - Login a user with an email and password. The password is verified against the hashed password stored in the database.</li>
</ul>

<h2>Validation</h2>
<p>User input is validated using Joi. The following validation rules are applied:</p>
<ul>
    <li><strong>Email</strong> - Must be a valid email address.</li>
    <li><strong>Password</strong> - Must be at least 5 characters long.</li>
</ul>




