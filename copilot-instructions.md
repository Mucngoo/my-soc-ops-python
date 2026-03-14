---
description: 'Workspace instructions for Soc Ops - a FastAPI + Jinja2 + HTMX social bingo game project'
---

# Soc Ops Workspace Instructions

## ✅ Mandatory Pre-Commit Checklist

Before pushing any changes:
1. **Lint**: uv run ruff check . — no errors
2. **Build**: uv run pytest — all 25 tests pass
3. **Test**: Open http://localhost:8000 in full browser, verify HTMX interactions

---

## Quick Start

`ash
uv sync                                                  # Install dependencies
uv run pytest                                           # Run tests
uv run uvicorn app.main:app --reload --port 8000      # Start dev server
`

**Prerequisites**: Python 3.13+, uv, full browser (Firefox/Chrome/Safari/Edge — not VS Code Simple Browser)

## Project Structure

- pp/main.py — FastAPI entry point
- pp/models.py — Pydantic models
- pp/game_service.py — Session management
- pp/game_logic.py — Core game mechanics
- pp/data.py — Game questions
- pp/templates/ — Jinja2 templates (HTMX powered)
- pp/static/css/app.css — Custom CSS utilities
- 	ests/ — 25 comprehensive tests
- workshop/ — Lab guides for extension

## Code Conventions

### Python
- Type hints required with Pydantic models
- Sessions via GameSession from game_service.py
- Tests in 	ests/test_*.py with pytest fixtures

### Frontend
- Jinja2 templates in pp/templates/
- CSS utilities in pp/static/css/app.css (see css-utilities.instructions.md)
- HTMX for dynamic interactions — **no Simple Browser**
- Components in pp/templates/components/

## Common Tasks

| Task | Steps |
|------|-------|
| Add game question | Edit pp/data.py → Update game_logic.py → Add test → Run uv run pytest |
| Create component | Create in pp/templates/components/ → Use CSS utils + HTMX → Include in template |
| Modify game state | Update pp/models.py → Update game_service.py → Update templates → Add tests |

## Architecture

**Backend**: FastAPI (Python 3.13+) with session middleware  
**Frontend**: Jinja2 + HTMX for real-time interactions (no page reloads)  
**Styling**: Custom utility CSS (Tailwind-like, no external dependencies)  
**Testing**: pytest covering game logic & API endpoints

## Important Rules

- ❌ Never use VS Code Simple Browser (HTMX requires full browser)
- ✅ Dev server auto-reloads on changes
- ✅ All game logic in pp/game_logic.py for consistency
- ✅ Validate inputs with Pydantic models

## Files & Links

| Instruction | Use When | Link |
|-------------|----------|------|
| setup.prompt.md | Dev environment setup | .github/prompts/ |
| general.instructions.md | General rules | .github/instructions/ |
| css-utilities.instructions.md | Styling work | .github/instructions/ |
| frontend-design.instructions.md | Frontend design | .github/instructions/ |

**FastAPI Docs**: http://localhost:8000/docs  
**HTMX Docs**: https://htmx.org  
**Jinja2 Docs**: https://jinja.palletsprojects.com

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Tests failing | uv sync, check 	ests/test_*.py, verify fixtures |
| HTMX not working | Use Firefox/Chrome/Safari/Edge (not Simple Browser), check console |
| Server not reloading | Restart: uv run uvicorn app.main:app --reload --port 8000 |

---

**Version**: 1.0 | **Updated**: March 2026
