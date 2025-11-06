This is my first try to FASTAPI personal project.

Frontend :- Refered to this video https://www.youtube.com/watch?v=Lu8lXXlstvM 
Project details
- Backend: FastAPI served with uvicorn
- Database: PostgreSQL (store credentials in DATABASE_URL / .env)
- Frontend: React app (separate frontend folder)

Quick start
1. Set environment variables (example):
```bash
export DATABASE_URL=postgresql://user:pass@localhost:5432/dbname
```
2. Install backend deps and run migrations (example):
```bash
pip install -r requirements.txt
# run your migration tool, e.g. alembic upgrade head
```
3. Start backend with uvicorn:
```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```
4. Start frontend:
```bash
cd frontend
npm install
npm start
```

Notes
- Ensure CORS is configured in FastAPI to allow the React dev server origin.
- Confirm Postgres is running and reachable before starting the app.