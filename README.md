# Kittygram Frontend

Kittygram is a simple web application for sharing and viewing cat profiles. This repository contains the frontend part of the project, built with React. The application allows users to register, log in, add new cats, edit and delete their own cats, and view a paginated list of all cats with their details and achievements.

> **Note:**  
> This project is provided as an example assignment for students. The main goal is for students to implement the backend API that will support this frontend. The frontend expects a RESTful API with endpoints for user authentication, cat management, and achievements.

## Features

- User registration and authentication (login/logout)
- Add, edit, and delete cat profiles (with image upload)
- Assign achievements to cats
- Paginated list of cats
- Responsive design
- Protected routes for authenticated users

## Technologies Used

- React (with hooks)
- React Router
- CSS Modules
- Fetch API for backend communication

## Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/boreesych/kittygram_frontend.git
cd kittygram_frontend
```

### 2. Install dependencies

```sh
npm install
```

### 3. Start the development server

```sh
npm run start
```

The app will be available at [http://localhost:3000](http://localhost:3000).

## Backend API

This frontend expects a backend API running at `http://127.0.0.1:8000`.  
You need to implement the backend API with the following endpoints:

- `POST /api/users/` — Register a new user
- `POST /api/token/login/` — Log in and receive an auth token
- `POST /api/token/logout/` — Log out the current user
- `GET /api/users/me/` — Get current user info
- `GET /api/cats/` — List cats (supports pagination)
- `POST /api/cats/` — Add a new cat
- `GET /api/cats/<id>/` — Get cat details
- `PATCH /api/cats/<id>/` — Edit a cat
- `DELETE /api/cats/<id>/` — Delete a cat
- `GET /api/achievements/` — List available achievements

The API should use token-based authentication.  
Refer to the frontend code in [`src/utils/api.js`](src/utils/api.js) for details on request formats and expected responses.

## Project Structure

```
kittygram_frontend/
├── public/
├── src/
│   ├── components/
│   ├── images/
│   ├── fonts/
│   ├── utils/
│   ├── index.js
│   └── index.css
├── package.json
└── README.md
```

## For Students

- Use this frontend as a client for your backend API.
- Make sure your backend endpoints match the expected URLs and data formats.
- You can extend the backend with additional features if desired.

## License

This project is for educational
