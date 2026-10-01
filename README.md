# EduGenie: Google Gemini Powered Learning Assistant

Features:
- AI educational Q&A
- Simple explanations
- Study-material summarization
- MCQ quiz generation
- Study-plan generation
- FastAPI backend
- Responsive web interface
- Gemini API integration with demo fallback

## Run

python -m venv edugenie-env
edugenie-env\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload

Open http://127.0.0.1:8000
API docs: http://127.0.0.1:8000/docs

Copy .env.example to .env and add GEMINI_API_KEY.
Without a key, the demo fallback still lets you demonstrate the application.


## Notes Module
EduGenie now includes a Notes module:
- Create a note with title and content
- View saved notes
- Delete notes
- Notes are exposed through `/api/notes`
