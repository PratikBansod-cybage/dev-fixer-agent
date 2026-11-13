---
name: coding-standards
description: Team Python coding standards. Use whenever you change Python code in this repository.
---

# Coding standards

- Add type hints to every function you change, including the return type.
- Keep each change minimal: fix the cause, don't refactor unrelated code.
- No print statements in library code; no bare `except:`.
- Run `python3 -m ruff check .` and fix every issue before you finish.
- Commit messages use: `fix(<TICKET>): <what changed, in the imperative>`.
