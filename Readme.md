# Full-Stack Interest Messaging Application

## Overview

This project is a full-stack application that allows users to send interest messages to other users. If the recipient accepts the interest, both users can chat with each other in real-time. The backend is built with Django, and the frontend is developed using React.

## Project Structure

- **Frontend**: A React application for user interface.
- **Backend**: A Django application providing the API and real-time chat functionality.

## Prerequisites and Dependencies

### Backend

- Python 3.8+
- Django 4.x
- Django Channels
- daphne (optional, for running the ASGI server)
- PostgreSQL (or any other database supported by Django)

### Frontend

- Node.js 14.x+
- React 18.x
- React Router
- WebSocket library (e.g., `stompjs` or native WebSocket API)

## Setup and Installation

### Backend

1. **Clone the Backend Repository**

   ```bash
   git clone https://github.com/yourusername/backend-repo.git
   cd backend-repo
