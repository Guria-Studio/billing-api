---
id: 20261029-fastapi-version-pin-ceiling-0-116-required
title: 'FastAPI version pin: ceiling <0.116 required'
area:
    - pyproject.toml
    - app/
tags:
    - fastapi
    - dependencies
    - pinning
source: agent
task: F0.T1
created: "2026-10-29"
---

Pin fastapi<0.116 in pyproject.toml — Starlette 1.0 (bundled with 0.116+) breaks the legacy TemplateResponse signature. The ceiling is load-bearing, not cosmetic.
