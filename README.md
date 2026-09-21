# Chess web application — coursework

A database and web-services project with a React frontend and Django backend. The original project describes chess openings and an unfinished game implementation.

## Repository layout

- `front/`: React client, package manifest and lockfile.
- `back/`: Django project and applications, migrations and Python requirements.
- `SQL/`: schema and query files.
- `Documentation/`: assignment documents and entity-relationship diagram.

## Local setup reference

These commands correct the folder names in the original README. Full application execution has not been revalidated, and the dependency manifests reflect the historical project.

Backend, from the repository root:

```sh
python -m venv .venv
# Activate .venv using your shell's activation command.
python -m pip install -r back/requirements.txt
cd back
python manage.py check
python manage.py migrate
python manage.py runserver 127.0.0.1:8000
```

Frontend, in a separate terminal:

```sh
cd front
npm ci
npm start
```

Inspect frontend API URLs and backend settings before running. Development setup is not a production deployment recipe; review credentials, authentication, origins and dependencies before exposing a server.

## Status

The chess game is incomplete. The original Heroku URL is historical and is not advertised as a working demo. Tracked Python bytecode was removed from the current tree; source, migrations, documents and the existing database were preserved. The database should be reviewed before reuse or publication of a new deployment.

[Portfolio](https://github.com/BadrEss01/BadrEss) · [Coursework index](https://github.com/BadrEss01/BadrEss/blob/main/COURSEWORK.md)
