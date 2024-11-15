# Flask Chat Application with Socket.IO

This Flask-based chat application allows users to create and join chat rooms with unique codes. Users can communicate in real-time through the chat rooms, and the app tracks messages and participants using Flask and Socket.IO.

## Features

- **Create/Join Chat Rooms**: Users can either create a new room or join an existing one by entering a unique room code.
- **Real-Time Messaging**: Using **Socket.IO**, users can send and receive messages instantly within the room.
- **Unique Room Codes**: Each room has a randomly generated code that ensures privacy and security.
- **User Sessions**: The app stores session information like the user's name and the room they are in to persist state across requests.

## Technologies Used

- **Flask**: A lightweight web framework for Python.
- **Flask-SocketIO**: For real-time communication between clients and server.
- **Sessions**: To store user-specific data such as name and room.
- **HTML/CSS**: For rendering the chat interface.

## Application Flow

1. **Home Page**: Users are prompted to enter their name and either create a new room or join an existing one by entering a room code.
2. **Room Page**: After creating or joining a room, users are redirected to the room page, where they can send and receive messages.
3. **Real-Time Communication**: Messages are broadcasted in real-time to all users in the room.
4. **Join/Leave Notifications**: When a user enters or leaves a room, a notification is sent to all users in the room.

## Setup and Deployment

### Requirements

- Python 3.x
- Flask
- Flask-SocketIO

### Installation

1. Install the necessary dependencies:


2. **Run the Application Locally**:

To run the application locally, execute:


3. **Deployment**:

- This application is ready for deployment on platforms like Render, Heroku, or any service that supports Python.
- For deployment, use **Gunicorn** as the WSGI server (recommended for production).


## Room and Chat Management

- **Creating/Joining a Room**: Users can create a new room or join an existing one by entering a unique room code. Rooms are stored in memory, and new rooms are generated with a 4-character unique code.
- **Real-Time Messaging**: When a user sends a message, it's immediately broadcast to all users in the room through Socket.IO.
- **User Sessions**: The app uses Flask sessions to store user data, ensuring that their room and name persist as they navigate the app.

## Dependencies

- `Flask`: Web framework for Python.
- `Flask-SocketIO`: Adds WebSocket support to Flask for real-time communication.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



