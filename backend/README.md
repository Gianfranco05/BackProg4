# Parcial Integrador Catálogo - Backend


## Requisitos
- Python 3.11+
- PostgreSQL en ejecución
- Base de datos creada, por ejemplo: `parcial_catalogo`

## Instalación
```bash
python -m venv .venv
source .venv/bin/activate  # En Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Variables de entorno
Crear un archivo `.env` a partir de `.env.example`.

Ejemplo:
```env
DATABASE_URL=postgresql+psycopg://postgres:TU_PASSWORD@localhost:5432/parcial_catalogo
APP_NAME=Parcial Integrador Catálogo
BACKEND_CORS_ORIGINS=http://localhost:5173,http://127.0.0.1:5173
SQL_ECHO=false
```

## Ejecutar el proyecto
```bash
uvicorn app.main:app --reload
```


## Documentación automática
- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`


## Notas
- Las tablas se crean al iniciar la aplicación con `SQLModel.metadata.create_all(...)`.
- Las relaciones muchos a muchos se resuelven con tablas puente.
- El archivo `.env` no debe subirse al repositorio.
- Completar en este README el enlace al video de la presentación antes de entregar.
