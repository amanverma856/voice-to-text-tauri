🎙️ Voice-to-Text Desktop App (Tauri + Deepgram)

A cross-platform Voice-to-Text desktop application built using Tauri and Deepgram Speech-to-Text API.
This project demonstrates how to capture microphone audio, process it, and convert speech into text in a desktop environment.

 Project Overview:

This application is a functional clone of Wispr Flow (core workflow).
The focus is on voice recording and accurate speech transcription, not UI design.

Users can:

Press a button to start recording

Speak through the microphone

Stop recording

Instantly see the transcribed text

 Tech Stack:

Tauri (v2) – Lightweight cross-platform desktop framework

Vanilla JavaScript – Frontend logic

HTML & CSS – Simple UI

Deepgram API – Speech-to-Text transcription

Web Media APIs – Microphone access and audio capture

 Features:

 Push-to-talk voice recording

 Microphone permission handling

 AI-powered speech-to-text (Deepgram)

 Displays transcribed text instantly

 Desktop app (Windows / macOS / Linux)

 Basic error handling

 Project Structure
voice-to-text-tauri/
├── src/
│   ├── index.html
│   ├── main.js
│   └── styles.css
├── src-tauri/
│   ├── src/main.rs
│   ├── Cargo.toml
│   └── .env (ignored)
├── README.md
└── package.json

 How It Works

The user clicks Start Recording

The app captures audio using the microphone

Audio is processed and converted to a supported format

Audio is sent to Deepgram Speech-to-Text API

Deepgram returns the transcribed text

The text is displayed in the app

 API Key Setup (Important)

This project uses the Deepgram API.

Create API Key

Go to https://console.deepgram.com/

Create a new API key

For Local Testing

The API key is used during development.
Do not commit your API key to GitHub.

Example:

Authorization: "Token YOUR_DEEPGRAM_API_KEY"

▶ Run the Project Locally
Prerequisites

Node.js

Rust

Tauri CLI

Windows/macOS/Linux system

Steps
npm install
npm run tauri dev

Demo Video

A short demo video is provided showing:

App startup

Recording voice

Transcription output

(Hosted on Google Drive / YouTube)

Known Limitations

UI is minimal (focus on functionality)

No background noise filtering

Single-language transcription (English)

API key handling can be further secured in backend

 Design Decisions:

Chose Tauri for lightweight desktop performance

Used Vanilla JS for simplicity

Focused on core voice-to-text workflow

Prioritized functionality over UI polish

 Future Improvements:

Move API key fully to backend

Add push-to-talk keyboard shortcut

Add language selection

Save transcription to file

Improve UI/UX

👤 Author

Aman kr Verma
B.Tech Graduate | Aspiring Software / AI Engineer

Assignment Checklist

 Desktop app using Tauri

 Microphone access

 Speech-to-text integration

 Working prototype
 
 Clean and readable code

 Documentation