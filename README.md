# WanderVoice AI 🌍🎙️

**WanderVoice AI** is an AI-powered travel guide that generates personalized travel information and converts it into natural-sounding audio guides.

## ✨ Features

- 🤖 **AI Travel Narratives** — Generate destination-specific travel information using Google Gemini.
- 🎙️ **AI Voice Guides** — Convert generated travel content into audio using Murf AI.
- 🌐 **Multi-language Support** — Generate travel guides in supported languages and voices.
- ⚡ **Interactive Web Interface** — Simple and responsive frontend for generating travel guides.
- 🔐 **Secure API Keys** — API credentials are managed through environment variables.

## 🏗️ Architecture

User
 │
 ▼
WanderVoice AI Frontend
 │
 │ REST API
 ▼
Flask Backend
 │
 ├──► Google Gemini API
 │       │
 │       └──► Travel Narrative
 │
 └──► Murf AI API
         │
         └──► Audio Guide


🛠️ Tech Stack

Frontend  : HTML5, CSS3, JavaScript
Backend   : Python, Flask, Flask-CORS
AI        : Google Gemini API, Murf AI API
Deployment: Vercel, Render
Tools     : Git, GitHub, VS Code

📁 Project Structure


WanderVoice-AI/
│
├── Backend/
│   ├── app.py
│   └── requirements.txt
│
├── Frontend/
│   ├── index.html
│   └── index.js
│
├── .gitignore
└── README.md


## ⚙️ Environment Variables

Create a `.env` file inside the `Backend` folder:


GOOGLE_API_KEY=your_gemini_api_key
MURF_API_KEY=your_murf_api_key


> **Never commit API keys or `.env` files to GitHub.**

## 🚀 Run Locally

### 1. Clone the repository

bash
git clone https://github.com/karthik309k/Travel-Guide-Using-MurfAI.git
cd Travel-Guide-Using-MurfAI


### 2. Install backend dependencies

bash
cd Backend
pip install -r requirements.txt


### 3. Start the Flask server

bash
python app.py


The backend will run on:

http://127.0.0.1:5000


### 4. Run the frontend

Open the `Frontend/index.html` file using **VS Code Live Server** or another local web server.

## 🌐 Deployment

- **Frontend:** Vercel
- **Backend:** Render
- **AI Services:** Google Gemini & Murf AI

## 🔄 Workflow

Enter Destination
       ↓
Select Guide Type / Language / Voice
       ↓
Frontend sends request to Flask API
       ↓
Gemini generates travel narrative
       ↓
Murf AI converts narrative to speech
       ↓
Audio + Transcript returned to user


## 🎯 Purpose

WanderVoice AI aims to make travel information more engaging by combining **generative AI with voice technology**, allowing users to experience destinations through personalized audio travel guides.

## 👨‍💻 Author

**Karthik**

GitHub: "https://github.com/karthik309k"

---

**Tech Stack:** HTML5 • CSS3 • JavaScript • Python • Flask • Google Gemini API • Murf AI • REST API • Git • GitHub • Vercel • Render
