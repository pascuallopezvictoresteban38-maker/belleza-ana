# Belleza Ana · Práctica 05

CRUD en Flask + MongoDB con API JSON (`/api/productos`).

## Antes de ejecutar
Copia la carpeta de Bootstrap de tu plantilla:
- `static/bootstrap/css/bootstrap.min.css`
- `static/bootstrap/js/bootstrap.bundle.min.js`

## Local (Windows)
    py -m venv .venv
    .\.venv\Scripts\python.exe -m pip install -r requirements.txt
    .\.venv\Scripts\python.exe app.py
Prueba la API (otra terminal): `.\.venv\Scripts\python.exe probar_api.py`

## Mac/Linux
    python3 -m venv .venv
    .venv/bin/python -m pip install -r requirements.txt
    .venv/bin/python app.py

## Render
Build: `pip install -r requirements.txt`
Start: `gunicorn app:app --bind 0.0.0.0:$PORT --workers 1 --threads 4 --timeout 60`
Variable: `MONGO_URI` (usuario de Atlas con readWrite solo en `belleza_ana`).
