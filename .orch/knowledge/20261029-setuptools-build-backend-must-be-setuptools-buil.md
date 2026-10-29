---
id: 20261029-setuptools-build-backend-must-be-setuptools-buil
title: setuptools build backend must be setuptools.build_meta
area:
    - pyproject.toml
tags:
    - setuptools
    - pyproject
    - build-backend
    - pip
source: agent
task: F0.T1
created: "2026-10-29"
---

The correct setuptools PEP 517 build backend is `setuptools.build_meta`, not `setuptools.backends.legacy:build`. The latter is invalid and causes `pip install -e .[dev]` to fail with a backend error. Always use `build-backend = "setuptools.build_meta"` in pyproject.toml.
