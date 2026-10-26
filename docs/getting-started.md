# Getting started

## Prerequisites

- Python 3.10 or newer
- pip

## Install

Run these commands from the `insurance_scheduler` project directory:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

If PowerShell blocks activation, use the virtual environment's interpreter
directly instead:

```powershell
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe app.py
```

## Run locally

Start the development server:

```powershell
python app.py
```

By default, it listens on `http://127.0.0.1:5000`. Visit `/` to check that the
API is running. The server uses Flask's built-in development server with debug
mode enabled; do not expose it as a production server.

## Current implementation

- `app.py` creates the Flask application and SQLAlchemy extension.
- SQLAlchemy is configured for a local SQLite database at
  `instance/scheduler.db`.
- No database tables, advisor/booking behavior, or automated tests are
  implemented yet.

