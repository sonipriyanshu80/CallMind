# CallMind Folder Stucture
callmind/
│
├── client/                  ← React frontend (UI)
│   ├── src/
│   │   ├── components/
│   │   │   ├── MicRecorder.jsx
│   │   │   ├── ChatBox.jsx
│   │   │   └── AudioPlayer.jsx
│   │   ├── App.js
│   │   └── api.js           ← Axios calls to Node backend
│   └── package.json
│
├── server/                  ← Node/Express backend
│   ├── app.js
│   ├── routes/
│   │   ├── upload.js        ← Receives audio
│   │   └── transcript.js
│   ├── controllers/
│   │   └── aiBridge.js      ← Sends data to Python AI backend
│   ├── models/
│   │   └── Conversation.js  ← Mongo schema
│   └── package.json
│
├── ai_core/                 ← Python AI engine
│   ├── app.py               ← Flask server
│   ├── stt.py               ← Whisper (Speech to Text)
│   ├── llm.py               ← GPT-5 (Text Generation)
│   ├── tts.py               ← Text to Speech
│   ├── requirements.txt
│   └── .env
│
├── .env                     ← global environment keys
└── README.md
