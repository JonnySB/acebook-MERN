# Acebook MERN

![acebook-overview](./gifs/acebook-overview.gig)

## What is Acebook?

Acebook is a Facebook clone developed using the MERN stack (MongoDB, Express.js
, React, & Node), with Tailwind CSS used for styling. It started life as a
group project in the Makers Software Engineering boot camp, where we were
provided with a small pre-existing codebase. Our task was to get up to speed
with an unfamiliar project structure and tech stack and then extend it based
on user requirements. After the project concluded, I continued to work on it
to further extend its functionality.

## Techologies used:

- MongoDB
- express.js
- React
- Node
- Tailwind

## Key learnings:

- MongoDB database architecture and design
- Model View Controler (MVC) design pattern
- MongoDB
- Express.js
- React component design and state management
- Cloud image hosting
- Creating modals
- TDD (React Testing Library)

## Setup

### Install Node.js

1. Install Node Version Manager (NVM)
   ```
   brew install nvm
   ```
2. Install the latest version of [Node.js](https://nodejs.org/en/)
   ```
   nvm install 20
   ```

### Set up your project

1. Clone repo one team member fork this repository
   ```
   git clone https://github.com/JonnySB/acebook-MERN.git
   ```
2. Install dependencies for both the `frontend` and `api` applications:
   ```
   cd frontend
   npm install
   cd ../api
   npm install
   ```
3. Install MongoDB
   ```
   brew tap mongodb/brew
   brew install mongodb-community@6.0
   ```
4. Start MongoDB
   ```
   brew services start mongodb-community@6.0
   ```

### Setting up environment variables.

We need to create two `.env` files, one in the frontend and one in the api.

#### Frontend

Create a file `frontend/.env` with the following contents:

```
VITE_BACKEND_URL="http://localhost:3000"
```

#### Backend

Create a file `api/.env` with the following contents:

```
MONGODB_URL="mongodb://0.0.0.0/acebook"
NODE_ENV="development"
JWT_SECRET="secret"
# CLOUD_NAME="<INSERT CLOUD NAME>"
# API_KEY="<INSET API KEY>"
# API_SECRET="<INSERT API SECRET>"
# CLOUDINARY_BASE_URL = "https://res.cloudinary.com/<INSERT CLOUD NAME>/image/upload/"
```

**NOTE - you will need to create a [cloudinary](https://cloudinary.com/) account for image uploads to work correctly.**

Once you have created an account, please update the details above.

### Run the server and use the app

1. Start the server application (in the `api` directory) in dev mode:

```
; cd api
; npm run dev
```

2. Start the front end application (in the `frontend` directory)

In a new terminal session...

```
; cd frontend
; npm run dev
```

# Things you could try:

- Sign-up as a user and login
  ![sign-up-and-login](/gifs/acebook-signup-and-login.gig)

- Add a profile picture (click the image icon on the profile page)
  ![add-profile-pic](/gifs/acebook-add-profile-pic.gif)

- Create a post
  ![create-post](/gifs/acebook-create-post.gif)

- Like and comment on a posts
  ![like-and-comment](/gifs/acebook-like-and-comment.gif)

- Visit your profile page and update bio information
  ![update-profile](/gifs/acebooke-update-profile.gif)
