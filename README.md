# Insurance Scheduler

A minimal Flask API starter for an insurance scheduling application. The current
API exposes a health-check endpoint; booking and advisor functionality has not
been implemented yet.

## Requirements

- Python 3.10 or newer
- pip

## Getting started

From the project directory, create and activate a virtual environment, then
install the dependencies:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Start the development server:

```powershell
python app.py
```

The server runs at `http://127.0.0.1:5000` by default. See
[Getting started](docs/getting-started.md) for setup details and
[API documentation](docs/api.md) for the available endpoint.

## Project structure

```text
insurance_scheduler/
├── app.py
├── docs/
├── models/
├── routes/
├── services/
└── requirements.txt
```

The application is initialized in `app.py`. SQLAlchemy is configured to use a
local SQLite database at `instance/scheduler.db`; no database models or
scheduling endpoints are implemented yet.

## Development

The Flask development server is configured with debug mode enabled. Use it only
for local development, not for production deployment.

