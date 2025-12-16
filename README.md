🎙️ Voice-to-Text Desktop App (Tauri + Deepgram)

A cross-platform AI-powered desktop application that converts voice input into text using Deepgram Speech-to-Text and Tauri.

This project is built as part of a technical assignment to demonstrate practical skills in desktop app development, audio processing, and AI API integration.

 Project Overview:

This application allows users to:

Press a button to start recording 

Speak naturally into the microphone

Stop recording

Instantly receive transcribed text 

The focus of this project is functionality, clean architecture, and secure API usage, not UI polish.

 Tech Stack:

Tauri (v2) – Lightweight, secure cross-platform desktop framework

Vanilla JavaScript – Frontend logic and UI interaction

Rust – Backend logic and secure API handling

Deepgram API – Speech-to-Text transcription

Web Audio API / MediaRecorder – Audio capture

 Core Features:

 Push-to-Talk Recording

 Microphone Permission Handling

AI-powered Speech-to-Text (Deepgram)

Cross-platform Desktop App

 Secure API Key Handling (Environment Variables)

Clean & Maintainable Code Structure

 Architecture Overview
Frontend (HTML + JS)
   |
   |  Audio Data
   v
Tauri Backend (Rust)
   |
   |  Secure API Call
   v
Deepgram Speech-to-Text API

Why this architecture?

API keys are never exposed in the frontend

Backend handles all third-party API communication

Follows real-world production standards

 API Key Security

Deepgram API key is stored in:

src-tauri/.env


The .env file is ignored via .gitignore

API key is accessed only in Rust backend

Frontend never contains secrets

Example .env file:

DEEPGRAM_API_KEY=your_api_key_here

 How to Run the Project Locally
1️ Prerequisites

Node.js (v18+ recommended)

Rust & Cargo

Tauri prerequisites installed

2️ Install dependencies
npm install

3️ Run the desktop app
npm run tauri dev

 How to Use the App:

Click Start Recording

Speak clearly into the microphone

Click Stop Recording

View the transcribed text in the text area

 Demo Video

A short demo video is included showing:

App launch

Voice recording

Real-time transcription

(Link provided in submission)

 Key Learnings & Challenges:

Handling microphone access across platforms

Debugging audio encoding issues on Windows

Securely managing API keys in desktop apps

Integrating real-time AI services into a native app

 Known Limitations

UI is minimal (focus was functionality)

No live streaming transcription (record-then-transcribe)

English language only (can be extended easily)

 Possible Enhancements

Push-to-talk keyboard shortcut

Multi-language support

Save transcription to file

Real-time streaming transcription

Improved UI/UX

 Author

Aman kr Verma
B.Tech Graduate | Aspiring Software & AI Engineer

✅ Final Notes

This project demonstrates:

Practical problem-solving

Clean separation of concerns

Secure API usage

Real-world desktop application development

Thank you!
