---
name: Day 1 backend scaffold
description: Day 1 backend scaffold is complete — structure, conventions, and runtime env details
type: project
---

Day 1 backend scaffold is implemented and tests pass at `project/backend/`.

**Why:** This is a 3-day sprint to build a markdown knowledge base (file-based, no DB). Day 1 goal was a runnable API with health check and config stub.

**How to apply:** Day 2 tasks are config loading, document CRUD, and validation. Pick up from this scaffold — do not restructure it.

Key facts:
- Python 3.12 venv lives at `project/backend/.venv/` — use `.venv/bin/pytest` and `.venv/bin/ruff`
- pip index includes a local mirror at `http://localhost:7999/simple/` (configured in the environment); pypi.org is also reachable
- `pyproject.toml` does NOT use a build backend (no hatchling/setuptools), so `pip install -e .` fails — install deps directly with pip
- `pytest-asyncio` mode is set to `auto` in `pyproject.toml` — no `@pytest.mark.asyncio` decorator needed
- API prefix is `/api/v1/`; health is at `/health` (no prefix)
- CORS origins are comma-separated in `CORS_ORIGINS` env var; `settings.cors_origins_list()` splits them
- Error shape for Day 2+: `{"error": string, "fields"?: Record<string, string>}`
