# demo-day

Savage Auth is the in-development codename for this demo day project.

# Savage Auth

A 21 Savage fan site that gives users a place to create an account, securely log in, and participate in a community message board. Authenticated users can view their profile, post messages, and interact with messages through upvote and downvote controls. The application uses Passport for local authentication, MongoDB for storing users and messages, Express sessions for persistent login sessions, and EJS templates for the front end.

If you use this product while it is still in development, please expect limited functionality and bugs as development continues. Bugs will be squashed!

## Tech Stack

* **Node.js:** Runtime environment for the application
* **Express.js:** Web server and routing framework
* **MongoDB:** Database for user and message data
* **Mongoose:** MongoDB object modeling
* **Passport.js:** Local email and password authentication
* **EJS:** Server-side HTML templating
* **Bootstrap 3:** Front-end layout and styling
* **CSS3:** Custom application styling
* **JavaScript (ES6+):** Client-side message interactions

## Features

* User signup with an email address and password
* Local user login and logout
* Persistent authenticated sessions
* Protected profile page
* Community message board
* Create new messages
* Upvote and downvote messages
* MongoDB-backed user and message data
* 21 Savage-themed home page and profile experience

## View on website

https://savage-auth-jvrw.onrender.com/



## How to run locally

http://localhost:8080

Have the following installed and configured:

* Node.js
* MongoDB Atlas account and database
* MongoDB network access configured for your development machine

## Installation

Clone the repository and move into the project directory:

```bash
git clone <repository-url>
cd savage-auth
```

Install the dependencies:

```bash
npm install
```

Create a `.env` file in the project root with the following:

```env
MONGODB_URI=mongodb+srv://<username>:<password>@<cluster-url>/<database-name>
```

Run the application:

```bash
node server.js
```

Then go to http://localhost:8080 in your browser to view the application.

## Available routes

* `/` — Home page
* `/login` — User login
* `/signup` — User registration
* `/profile` — Authenticated profile and message board
* `/logout` — Log out of the current session

## Environment and local files

Ensure that `.gitignore` contains:

```text
.env
node_modules
.DS_Store
```

`.DS_Store` is only needed if you are running the project locally on macOS.

## Project structure

```text
app/
  routes.js
  models/
    user.js
config/
  database.js
  passport.js
public/
  main.js
  style.css
  img/
views/
  connect-local.ejs
  index.ejs
  login.ejs
  profile.ejs
  signup.ejs
server.js
Procfile
```

## Credits

Modified from the Scotch.io authentication tutorial.
