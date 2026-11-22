# Nocturne Coach

An AI piano practice coach for beginner and intermediate students. It builds
personal practice plans, helps with difficult passages, and tracks daily progress.

**Live app:** [paste your Streamlit link here]

## Features
- Profile sidebar (level, current piece, minutes per day, goal)
- Practice plans as a table (Task, Minutes, Tempo/Focus)
- Daily plan tracker with progress bar and practice streak
- Export the plan as a text file
- Quick-prompt buttons for common questions
- Upload practice notes as a .txt file

## Prompt defenses
- XML tagging: uploaded notes are wrapped in tags and treated as untrusted data
- Input filtering: .txt uploads only, length limits, and a warning for instruction-like text
- Instruction defense: the system prompt is confidential and refuses persona changes

## Run locally
1. Clone this repository and open the folder.
2. (Optional) Create and activate a virtual environment.
3. Install the dependencies: `pip install -r requirements.txt`
4. Add your Gemini API key as an environment variable or in `.streamlit/secrets.toml`:
   ```toml
   GEMINI_API_KEY = "your-key-here"
   ```
5. Start the app: `streamlit run app.py`

Never commit your real API key. `.streamlit/secrets.toml` is listed in `.gitignore`.

## Tech
Streamlit, Google Gemini (google-genai SDK)

## Team
[Member names]
