# TIC TAC TOE (Django)
A simple Tic-Tac-Toe game with a Django backend and a lightweight front-end.  

## Tech Stack
**Frontend**
- HTML5 templating (Django Template Language)
- CSS3 (vanilla)
- JavaScript (vanilla) + Fetch API

**Backend**
- Python 3
- Django 4.2 (MVT)
- JSON endpoints: `/move/<int:pos>/`, `/restart/`

**Database**
- SQLite (development default)

## How it works
- The UI is rendered with a Django template and static assets.
- Clicks on the board call the Django JSON endpoints via `fetch()`.
- Server-side game logic in `game/logic.py` updates state, checks win/tie, and returns the board + status.

### Migrate & run
- python manage.py migrate
- python manage.py runserver

Open http://127.0.0.1:8000/
