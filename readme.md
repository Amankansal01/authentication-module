# Node.js Authentication API

A simple authentication API built with Node.js, Express, and MongoDB, featuring JWT-based auth and secure password hashing with bcrypt.

## Setup & Installation

- Clone the repository:

```bash
  git clone https://github.com/Amankansal01/authentication-module.git
  cd authentication-module
```
    
- Install dependencies:

```bash
  npm install
```
- Configure environment variables: Create a .env file at the root level and add the following variables:

```bash
PORT=4000
CORS_ORIGIN =*
MONGO_URI=<Your MongoDB URI>
ACCESS_TOKEN_SECRET=<YourACCESS_TOKEN_SECRETkey>
ACCESS_TOKEN_EXPIRY=1d
  

```
    
- Run in Development:

```bash
  npm run dev
```

The server should now be running at `http://localhost:4000`
## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`PORT`
`CORS_ORIGIN`
`MONGO_URI`
`ACCESS_TOKEN_SECRET`
`ACCESS_TOKEN_EXPIRY`


## Features

- User registration & login
- JWT-based authentication
- Cookie-based logout
- Protected route to fetch current user
- Environment-based configuration
- CORS enabled


## API Endpoints

| Method | Route                  | Description           |
|--------|------------------------|-----------------------|
| POST   | `/api/auth/register`   | Register a new user   |
| POST   | `/api/auth/login`      | Login and get token   |
| POST   | `/api/auth/logout`     | Logout user           |
| GET    | `/api/auth/current-user` | Get logged-in user info (requires token) |




