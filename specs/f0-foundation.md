# F0 — Foundation

## T1 — Scaffold FastAPI project layout

- `pyproject.toml` with `[build-system] requires = ["setuptools>=68"]`,
  `build-backend = "setuptools.build_meta"`, and
  `[tool.setuptools] packages = ["app"]`.
- Check it the way CI does, in a throwaway venv in the worktree (never the
  system Python): `python3 -m venv .venv && .venv/bin/pip install -q -e .[dev]
  && .venv/bin/pytest -q`. `.venv/` is gitignored.
- Add `tests/test_import.py` asserting `from app.main import app` works, so CI
  has a test to run.
