---
name: test-conventions
description: Team rules for tests. Use whenever you fix a bug or add or change tests.
---

# Test conventions

- Every bug fix adds a regression test named `test_<function>_regression_<ticket>` (ticket in lower case, e.g. `test_add_regression_scrum_1`) in the matching `tests/test_<module>.py`.
- Use `pytest.mark.parametrize` when a test checks three or more cases; include at least one negative number and zero.
- Never delete, skip or weaken an existing test to make a fix pass.
- Run tests with `python3 -m pytest -q` and report the summary line.
