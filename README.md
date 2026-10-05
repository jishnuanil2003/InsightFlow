# InsightFlow

Agentic AI system that performs data analysis from natural-language queries over uploaded CSV/Excel files, and produces evidence-backed reports.

**Stack:** LangGraph, LangChain, Gemini/GPT, Pydantic, DuckDB, Pandas, FastAPI, PostgreSQL, React, Vite, Tailwind, LangSmith.

## Layout
- `backend/` FastAPI + LangGraph agents + tools
- `frontend/` React + Vite UI (15% chats / 60% analysis / 25% uploads)
- `docs/` architecture notes

## Quick start
```bash
cp .env.example .env
docker compose up -d
cd backend
python -m venv .venv && source .venv/bin/activate
pip install -e ".[dev]"
uvicorn app.main:app --reload
pytest
```

## Status
Phase 1 in progress: text-only analysis agent (no charts, no persistent memory).
