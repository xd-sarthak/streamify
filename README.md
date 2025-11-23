# Streamify Video Calls

Streamify Video Calls is a full-stack web application enabling real-time video calls, chat, and social features. It is built with a Node.js/Express backend and a React/Vite frontend, supporting user authentication, friend management, notifications, and more.

## Features

- **User Authentication:** Sign up, login, logout, and onboarding flows.
- **Video Calls:** Initiate and join video calls with friends.
- **Chat System:** Real-time messaging between users.
- **Friend Management:** Send, accept, and reject friend requests.
- **Notifications:** Receive notifications for friend requests and other events.
- **Theme Selection:** Switch between light and dark modes.
- **Responsive UI:** Modern, mobile-friendly design using Tailwind CSS.

## Project Structure

```
streamify-video-calls/
	backend/      # Node.js/Express API server
	frontend/     # React/Vite client app
```

## Backend API Endpoints

### Auth Routes (`/api/auth`)
- `POST /api/auth/signup` — Register a new user.
- `POST /api/auth/login` — Authenticate and login.
- `POST /api/auth/logout` — Logout the current user.
- `GET /api/auth/me` — Get current authenticated user info.

### User Routes (`/api/users`)
- `GET /api/users` — List all users.
- `GET /api/users/:id` — Get user by ID.
- `POST /api/users/friend-request` — Send a friend request.
- `POST /api/users/friend-request/accept` — Accept a friend request.
- `POST /api/users/friend-request/reject` — Reject a friend request.
- `GET /api/users/notifications` — Get user notifications.

### Chat Routes (`/api/chat`)
- `GET /api/chat/:friendId` — Get chat history with a friend.
- `POST /api/chat/send` — Send a chat message.

### Video Call/Stream Routes (`/api/stream`)
- `POST /api/stream/start` — Start a video call/stream.
- `POST /api/stream/join` — Join an existing video call/stream.

## Frontend

- Built with React and Vite.
- Uses Tailwind CSS for styling.
- Components for calls, chat, friends, notifications, and theme selection.
- Custom hooks for authentication and API integration.

## Getting Started

### Backend

```bash
cd backend
npm install
npm start
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

## Environment Variables

Both `backend/.env` and `frontend/.env` files are used for configuration. Set your API URLs, secrets, and other environment-specific settings here.

## License

MIT
