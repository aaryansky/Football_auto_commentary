# AutoCommentary — AI-Powered Football Match Commentary 🎙️⚽

A full-stack FastAPI + React project that detects football match events and generates AI commentary.

## Features
- Upload football match clips
- Background processing pipeline (`run_pipeline`)
- Generates structured event JSON
- TTS placeholders (to be upgraded to real audio)
- REST API: `/upload/`, `/api/events/{match_id}`

## Project Structure

auto_commentry/
│
├── backend/
│ ├── app/
│ │ ├── main.py
│ │ ├── api/
│ │ │ └── routes.py
│ │ └── services/
│ │ └── vision.py
│ ├── data/ (auto-created)
│
├── frontend/
│ └── (React app)
│
├── data/ (auto-created)
└── .venv/ (ignored)

## Running the Backend
```bash
uvicorn backend.app.main:app --reload --port 8000