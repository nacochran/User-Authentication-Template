# User Authentication Template
Template for local & 3rd party authentication for user accounts, using JavaScript, Node, Express, Passport, and PostgreSQL.

## Setting Up App

### 1. Install Dependencies
Use `npm install` to install all required node packages in package.json.

### 2. Configure Google Credentials
Go to [Google Cloud Console](https://console.cloud.google.com/) and either create a new project or select an existing one. 
Then navigate to the credentials page and access your OAuth clientID and OAuth secret.

### 3. Set Environment Variables
Create a `.env file` in the root of your project and add the following information:
<pre>
GOOGLE_CLIENT_ID=YOUR_GOOGLE_CLIENT_ID
GOOGLE_CLIENT_SECRET=YOUR_GOOGLE_CLIENT_SECRET
SESSION_SECRET=KEY_FOR_BCRYPT
PG_USER="postgres"
PG_HOST="localhost"
PG_DATABASE="secrets"
PG_PASSWORD="password for your database"
PG_PORT="5432"
</pre>

### 4. Run application
Use `node app.js` or `nodemon app.js` to run your project.

### 5. View Application
The app runs on port 3000 by default. Go to localhost/3000 to view the app.
