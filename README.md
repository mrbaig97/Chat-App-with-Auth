# Chat App Backend

## Description
This repository contains the backend implementation for a chat application built using Node.js and Express.js. The backend facilitates real-time messaging, user authentication, and chat management.

## Features
- Real-time messaging using WebSocket (Socket.IO)
- User authentication and authorization
- Chat creation and management
- Message history retrieval
- Delete messages functionality (for self and everyone)

## Technologies Used
- Node.js
- Express.js
- MongoDB (using Mongoose)
- Socket.IO for real-time communication
- JSON Web Tokens (JWT) for user authentication

## Setup Instructions
1. **Clone the Repository:**
   ```bash
https://github.com/mrbaig97/Chat-App-with-Auth.git
   cd chat-app-backend
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root of the project and set the following variables:
   ```env
   PORT=3000
   MONGODB_URI=mongodb://localhost:27017/chat_app
   JWT_SECRET=your-secret-key
   ```

4. **Run the Application:**
   ```bash
   npm start
   ```

5. **API Endpoints:**
   - `POST /api/auth/login`: User login
   - `POST /api/auth/register`: User registration
   - `GET /api/message/chat-list`: Get the list of chats
   - `GET /api/message/:user`: Get messages for a specific user
   - `POST /api/message/send`: Send a new message
   - `DELETE /api/message/delete-for-me/:messageId`: Delete a message for the current user
   - `DELETE /api/message/delete-for-everyone/:messageId`: Delete a message for everyone (permission required)

## Socket.IO Events
- `connection`: Event emitted when a client connects
- `disconnect`: Event emitted when a client disconnects
- `message`: Event emitted when a new message is received

## Contributing
Contributions are welcome! Feel free to open issues and pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Express.js](https://expressjs.com/)
- [Socket.IO](https://socket.io/)
- [Mongoose](https://mongoosejs.com/)
- [JSON Web Tokens](https://jwt.io/)

## Contact
For any inquiries, please contact farazbaig521@gmail.com.
