# TalentScout — AI Hiring Assistant 

AI-powered tools to help recruiters and educators move faster:

A Streamlit chatbot that runs an initial candidate screen, asks context-aware technical questions with Google Gemini, and saves results.

A lightweight Flask API that scores written assignments with Gemini, generates rubrics/model answers on the fly, and flags plagiarism against peer submissions.

The app uses the Gemini model models/gemini-2.0-flash-lite and reads your API key from .env

# Features

Conversational screening flow (name, email, phone, experience, role, location → tech stack → targeted questions). State is handled explicitly via constants. 
GitHub
+1

Tech-aware questions: questions are generated from the candidate’s stated stack (Python/React/AWS/etc.), with up to 3 questions per tech. 
GitHub
+1

Persisted results: candidate records (profile + Q&A) are saved to data/candidates.json. A sample file is already present. 
GitHub
+1

Assignment API: POST /api/evaluate returns structured feedback, numeric score JSON (when available), and plagiarism info. Endpoints to fetch generated model answers and rubrics are also included.
