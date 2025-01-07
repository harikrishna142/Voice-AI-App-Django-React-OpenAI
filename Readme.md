# An AI Assistant with chat, voice capabilties using state of the art LLM, STT, TTS functionalities
## Description
 A full-stack web application developed with django as backend, react native as frontend with tailswind css. The Assiatnt integrated with LLM suchas Open AI, Gemini, Claude, And for sppech to text deepgrams nova-2 modle is used, and elevenlabs API for text to speech.


## Demo
![Super-Voice-Assistant Demo](https://github.com/hounfodji/Super-Voice-Assistant/blob/master/z_demo/demo.png)
*Caption: Super-Voice-Assistant in action, showing the voice recording interface and AI response.*


## Features
- Audio recording and playback
- Speech-to-text conversion
- AI-powered responses
- Text-to-speech output
- Real-time chat interface
## Prerequisites
Before you begin, ensure you have met the following requirements:
- **Python 3.x:** Download and install from [python.org](https://www.python.org/downloads/)
- **Node.js and npm:** Download and install from [nodejs.org](https://nodejs.org/)
- **Git:** Download and install from [git-scm.com](https://git-scm.com/)
## Installation
### Backend (Django)
1. Clone the repository:
   ```bash
   git clone https://github.com/hounfodji/Super-Voice-Assistant.git
   cd Super-Voice-Assistant
   ```
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up your environment variables:
   Create a `.env` file in the root directory and add your AI API key:
   Get Gemini API key [here](https://aistudio.google.com/app/apikey)
   ```
   GEMINI_API_KEY=your_api_key_here
   ```
5. Run migrations:
   ```bash
   python manage.py migrate
   ```
6. Start the Django development server:
   ```bash
   python manage.py runserver
   ```
### Frontend (React)
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install the required npm packages:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm run dev
   ```
## Usage
1. Open your web browser and go to `http://localhost:5173` to access the React frontend.
2. Click the "Start Recording" button to begin recording your voice.
3. Speak your query or command.
4. Click "Stop Recording" when you're done speaking.
5. The application will process your audio, convert it to text, send it to the AI for processing, and display the response.
6. The AI's response will be displayed in the chat interface and spoken aloud.
## API Endpoints
- `POST /api/record/`: Accepts audio recordings and returns the transcribed text.
- `POST /api/process/`: Accepts text input and returns the AI-generated response.
