# AGENTS.md

Greenfield repo: coursework codebase for "115-1 computer programming". Currently only `README.md`, `LICENSE` (MIT), and a standard Python `.gitignore`. No source, no build/test/lint config, no CI.

- 回應語言：所有回應一律使用繁體中文。
- 程式語言：本專案使用 Python。
- 套件管理：一律使用 conda 管理 Python 套件，不要使用 pip / venv / uv / poetry。
- Conda 環境：`iem_python`。安裝套件或執行程式前，先確認已進入此環境（`conda activate iem_python`），或使用 `conda run -n iem_python ...`。
- 尚未固定 `pyproject.toml` / `requirements*.txt` / `pytest.ini` 等設定。不要假設已存在；如需新增相依套件，先確認並以 conda 方式安裝，不要擅自引入框架或測試執行器。
- `.gitignore` already covers Python defaults (`__pycache__/`, `*.py[codz]`, `.venv`/`venv/`/`env/`, `.pytest_cache/`, `.ruff_cache/`, `.mypy_cache/`). Do not commit those.
- Prefer plain stdlib Python scripts until the repo establishes a convention. Keep new code self-contained per assignment unless the user asks for shared packaging.
- 驗證方式：目前沒有測試套件，執行 `conda run -n iem_python python <file.py>` 驗證。
