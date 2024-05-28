# ChatGPT Clone

This repository contains a Django-based web application that simulates a ChatGPT-like chatbot interface. The application allows users to interact with the chatbot, view chat history, and handle file uploads for processing input.

## Features

- **Chat Interface**: Users can input messages and receive responses from the chatbot.
- **Chat History**: Users can view previous chat sessions and delete individual entries.
- **File Upload**: Users can upload documents, which the chatbot will read and use to generate responses.
- **Responsive Design**: The UI is built to be responsive and user-friendly.

## Project Structure

### Templates

#### `index.html`
The main HTML template for the application. It includes:

- A side panel to toggle and view chat history.
- The chat container to display user and bot messages.
- A form to handle new chat inputs and file uploads.

### Views

#### `views.py`
Contains the view functions to handle various aspects of the application:

- `index(request)`: Renders the main index page with chat history.
- `user_inp(request)`: Processes user input from the chat form.
- `delete_entry(request, entry_id)`: Deletes a specific chat entry.
- `single_entry(request, entry_id)`: Displays a specific chat entry.
- `new_chat(request)`: Starts a new chat session while retaining the old chat history.
- `out(request)`: Handles the main chat interaction logic, including processing file uploads and saving chat history.

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/chatgpt-clone.git
    cd chatgpt-clone
    ```

2. **Create a virtual environment and activate it**:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Run database migrations**:
    ```sh
    python manage.py migrate
    ```

5. **Start the development server**:
    ```sh
    python manage.py runserver
    ```

6. **Access the application**:
    Open your web browser and go to `http://127.0.0.1:8000/`.

## Usage

- **Chatting**: Enter your message in the chat input field and press send. The bot will respond to your message.
- **Chat History**: Click the "Chat History" button to view past chats. You can click on a chat entry to view it or delete it using the delete button.
- **File Upload**: Use the attach button to upload a document. The bot will process the content of the document and respond accordingly.


##Output
![1](https://github.com/MuhammedAshiqu/chatgpt-clone/assets/69718823/a605c6ae-fc79-43f9-8448-49ddc66e6ab1)
![2](https://github.com/MuhammedAshiqu/chatgpt-clone/assets/69718823/0ec3a22d-6aab-483f-8c59-a11b41e03653)
![3](https://github.com/MuhammedAshiqu/chatgpt-clone/assets/69718823/b5b46c35-9912-4b8d-9c5a-fb4046c177db)

