# Project Issues

Tracking issues identified during development and testing.

## Completed Tasks

- [x] Fix `ModuleNotFoundError` in test files.
- [x] Prevent `pytest` from collecting tests in `backup/` directory.
- [x] Verify `SyntaxWarning: invalid escape sequence` is resolved in `tests/test_config.py`.

## In Progress Tasks

- None

## Future Tasks

- None

## Implementation Plan

1.  ~~**Fix Imports:** Update all `import` statements in `Git_Auto_commit_Pip-Project/tests/*.py` to use `git_auto` instead of `git_auto_commit`.~~ (Done)
2.  ~~**Configure Pytest:** Add `norecursedirs = backup` to `pyproject.toml` under `[tool.pytest.ini_options]` to stop pytest from looking inside the `backup` folder.~~ (Done)
3.  ~~**Verify Raw Strings:** Double-check `tests/test_config.py` to ensure all regex patterns use raw strings (`r"..."`).~~ (Done)
4.  **Re-run Tests:** Instruct user to clean environment and re-run `pytest` from the project root.

### Relevant Files

- `Git_Auto_commit_Pip-Project/tests/test_ai_interface.py` - ✅ Needs import path update.
- `Git_Auto_commit_Pip-Project/tests/test_cli.py` - ✅ Needs import path update.
- `Git_Auto_commit_Pip-Project/tests/test_config.py` - ✅ Needs import path update & raw string verification.
- `Git_Auto_commit_Pip-Project/tests/test_git_utils.py` - ✅ Needs import path update.
- `Git_Auto_commit_Pip-Project/tests/test_sanitizer.py` - ✅ Needs import path update.
- `Git_Auto_commit_Pip-Project/tests/test_validation.py` - ✅ Needs import path update.
- `Git_Auto_commit_Pip-Project/pyproject.toml` - ✅ Needs pytest configuration update.
