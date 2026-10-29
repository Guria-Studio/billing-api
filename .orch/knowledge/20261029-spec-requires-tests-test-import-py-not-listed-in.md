---
id: 20261029-spec-requires-tests-test-import-py-not-listed-in
title: Spec requires tests/test_import.py not listed in task files
area:
    - tests/
    - specs/
tags:
    - spec
    - tests
    - files
source: agent
task: F0.T1
created: "2026-10-29"
---

The spec (specs/f0-foundation.md#T1) requires adding tests/test_import.py for CI to have a test to run, but it was not listed in the task's `Files you may write`. Future tasks should check the spec ref for extra required files beyond the listed ones and add them, noting the reason in the done note.
