# Client-Server Chatbot

A simple client-server chatbot application using Python sockets and Flask, powered by the Groq API.

## Features
- Real-time chat between client and server
- AI-powered responses using Groq API
- Web interface for chatting
- Environment variables for API keys and endpoints

## Project Structure
```
├── client.py           # Client-side socket code
├── server.py           # Server-side socket and Flask web app
├── templates/
│   └── chat.html       # Web chat interface
├── .env.example        # Example environment variables
├── .gitignore          # Files to ignore in version control
```

## Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/mo-elgazar74/Client-Server-Chatbot.git
   cd Client-Server-Chatbot
   ```
2. **Install dependencies**
   ```bash
   pip install flask python-dotenv requests
   ```
3. **Configure environment variables**
   - Copy `.env.example` to `.env` and fill in your Groq API key and URL:
     ```
     GROQ_API_KEY=your_actual_api_key
     GROQ_API_URL=https://api.groq.com/openai/v1/chat/completions
     ```

## Running the Project
1. **Start the server**
   ```bash
   python server.py
   ```
   ```bash
   python client.py
   ```
2. **Access the web interface**
   - Open your browser and go to `http://127.0.0.1:5000`

## Deployment Notes
- Ensure your `.env` file is present and contains valid API keys on your server.
- For production, use a WSGI server (e.g., Gunicorn) and a reverse proxy (e.g., Nginx).
- Never commit your real `.env` file or API keys to public repositories.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
