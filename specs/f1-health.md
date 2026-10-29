# F1 — Health

## T1 — Health endpoint + integration test

- `GET /health` returns `{"status": "ok"}` with 200.
- `tests/test_health.py` uses `fastapi.testclient.TestClient`.
- Run it as CI does: `python3 -m venv .venv && .venv/bin/pip install -q -e .[dev]
  && .venv/bin/pytest -q` (never the system Python).
