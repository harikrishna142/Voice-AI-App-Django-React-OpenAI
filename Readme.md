# An AI Assistant with chat, voice capabilties using state of the art LLM, STT, TTS functionalities
## Description
Super-Voice-Assistant is a full-stack web application that creates a customizable voice assistant. It combines a Django backend with a React frontend, allowing users to interact with an AI-powered assistant through audio recordings. The application leverages the power of a chosen AI solution (e.g., Gemini or others) to foster engaging conversational experiences.

## Demo
![Super-Voice-Assistant Demo](https://github.com/hounfodji/Super-Voice-Assistant/blob/master/z_demo/demo.png)



## Features
- Audio recording and playback
- Speech-to-text conversion
- AI-powered responses
- Text-to-speech output
- Real-time chat interface

### Backend 
1. Clone the repository:
   
3. pip install -r requirements.txt
   
4. set up GEMINI_API_KEY=your_api_key_here
   
5. python manage.py migrate


6. 
   python manage.py runserver
   ```
### Frontend (React)
1. cd frontend
   
2. npm install
   
3.npm run dev
  
## Usage
1. Open your web browser and go to `http://localhost:5173` to access the React frontend.
2. Click the "Start Recording" button to begin recording your voice.
3. Speak your query or command.
4. Click "Stop Recording" when you're done speaking.
5. The application will process your audio, convert it to text, send it to the AI for processing, and display the response.
6. The AI's response will be displayed in the chat interface and spoken aloud.



