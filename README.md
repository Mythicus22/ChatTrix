# Chat Application

A modern web-based chat platform that enables seamless communication between users and integrates an AI-powered assistant using Google's Gemini API. Built with Node.js and Express.js, this application provides a secure, responsive interface for both interpersonal messaging and intelligent conversations.

## Features Breakdown

### User Authentication
- Secure registration and login system
- Password hashing using bcrypt
- Session-based authentication

### Messaging System
- User-to-user private messaging
- Message read status tracking
- Contact list management
- Real-time message updates

### AI Chat Integration
- Integration with Google's Gemini API
- Multiple chat sessions support
- Session management and history
- Smart conversation context handling

## Security Features
- Password hashing
- Session management
- HTTP-only cookies
- Input validation
- Environment variable protection
- Authentication middleware

- **User Authentication**: Secure registration and login system with password hashing
- **User-to-User Messaging**: Real-time chat functionality with message read status tracking
- **AI Chat Assistant**: Interactive conversations powered by Google's Gemini API with support for multiple chat sessions
- **Session Management**: Persistent chat sessions with the ability to create, switch, and manage multiple AI conversations
- **Responsive Design**: Mobile-friendly interface built with EJS templates and custom CSS
- **Flash Notifications**: User feedback system for successful actions and error handling
- **Contact Management**: User directory for easy messaging with other registered users

## Technology Stack

### Backend Implementation
- **Node.js & Express.js**: Server-side framework for handling HTTP requests, routing, and middleware
- **MongoDB & Mongoose**: NoSQL database for storing user data, messages, and chat sessions with schema validation
- **Express-Session**: Server-side session management for user authentication state
- **bcrypt**: Password hashing for secure user authentication
- **Connect-Flash**: Temporary message storage for user notifications

### Frontend Implementation
- **EJS & EJS-Mate**: Templating engine for dynamic HTML generation and layout management
- **CSS**: Custom styling for responsive, user-friendly interface

### AI Integration
- **Google Gemini API**: Advanced language model integration for AI chat functionality with configurable safety settings and generation parameters

## Prerequisites

- Node.js (v18 or higher)
- MongoDB (Atlas cloud or local instance)
- Google Gemini API key

## Environment Setup

Configure the following environment variables in a `.env` file:

```
Mongo_URL=your_mongodb_connection_string
GEMINI_API_KEY=your_gemini_api_key
NODE_ENV=development
```

## Usage

1. Start the server: `npm start`
2. Access the application in your web browser
3. Register a new account or log in
4. Navigate to chat features for user messaging or AI conversations

## Contributing

Contributions are welcome. Please fork the repository and submit a pull request with your improvements.

## License

ISC License
```

## API Endpoints

- `GET /` - Landing page
- `GET /login` - Login page
- `POST /login` - Authenticate user
- `GET /register` - Registration page
- `POST /register` - Create new user
- `GET /home` - Home page (authenticated)
- `GET /logout` - Logout user
- `GET /chat` - User chat interface
- `POST /chat/send` - Send message to user
- `GET /ai` - AI chat interface
- `POST /ai/chat` - Send message to AI
- `POST /ai/new` - Create new AI chat session
- `GET /ai/session/:sessionId` - Switch AI chat session

## License

This project is licensed under the ISC License.

## Acknowledgments

- Google Gemini API for AI chat functionality
- MongoDB for database services
- Express.js community for the web framework
   ```powershell
   # Windows (PowerShell)
   $env:GEMINI_API_KEY = "your_key_here"
   ```

## Project Structure

```
chat-app/
├── app.js              # Main application file
├── models/             # Database models
│   ├── aichat.js      # AI chat model
│   ├── message.js     # Message model
│   └── user.js        # User model
├── public/            
│   └── style.css      # Application styles
├── views/             # EJS templates
│   ├── ai.ejs         # AI chat interface
│   ├── chat.ejs      # User chat interface
│   ├── home.ejs      # Home page
│   ├── land.ejs      # Landing page
│   ├── login.ejs     # Login page
│   ├── register.ejs  # Registration page
│   ├── includes/     # Reusable components
│   └── layout/       # Page layouts
└── package.json       # Project dependencies
```

## License

This project is licensed under the ISC License.

## ⚠️ Note on Repository History

This project was originally developed by me on my previous GitHub account (Devansh2835), which I lost access to due to 2FA issues.

The original repository can be found here: https://github.com/Devansh2835/chat-app.git

This is a re-upload for portfolio purposes.

