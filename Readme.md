# Full-Stack Messaging Application

## Overview

This project is a full-stack application that allows users to send interest messages to other users. If the recipient accepts the interest, both users can chat with each other in real-time. The backend is built with Django, and the frontend is developed using React.

## Project Structure

- **Frontend**: A React application for user interface.
- **Backend**: A Django application providing the API and real-time chat functionality.

## Prerequisites and Dependencies

### Backend

- Python 3.8+
- Django 4.2
- Django Channels
- daphne 
- SQLITE (or any other database supported by Django)

### Frontend

- Node.js 14.x+
- React 18.x
- React Router
- WebSocket library (e.g., `stompjs` or native WebSocket API)

## Setup and Installation

### Backend

1. **Clone the Backend Repository**

   ```bash
   git clone https://github.com/rohandass58/Interesting_Chat_Application.git
   cd chat_app
   ```

2. **Create and Activate a Virtual Environment**

    ``` bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```


3. **Install Dependencies**
   ```bash
      pip install -r requirements.txt
   ```
4. **Apply Migrations**
   ```bash
      python manage.py makemigrations
      python manage.py migrate
   ```
5. **Run Backend Server **
   ```bash
      daphne -b 0.0.0.0 -p 8000 interest_app_backend.asgi:application
   ```

## Frontend

1. **Move to the Frontend Directory**
   ```bash
      cd my-frontend
   ```
2. ** Install Dependencies**
   ```bash
      npm install
   ```
3. **Start the Development Server**
   ```bash
   npm start
   ```
   The frontend should now be available at http://localhost:3000.


## How to Run the Application

1. **Register and Login**

   - **Register**: Use a mobile number and password to register a new account.
   - **Login**: Log in with your mobile number and password.

2. **Browse Users**

   - After logging in, you can see a list of users to whom you can send an interest message.

3. **Send and Manage Interests**

   - **Send Interest**: Send an interest message to other users.
   - **Manage Interests**: View received interest messages and accept or reject them.

4. **Start Chatting**

   - If an interest is accepted, you can start chatting with the user. Open the chat interface and send/receive messages in real-time.
