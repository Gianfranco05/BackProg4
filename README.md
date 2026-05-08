# Parcial 1 

## Integrantes
- Lucas Pujada
- Gianfranco Canciani
- Julio Leiva
- Bruno Rivera


### Crear la base de datos
Antes de ejecutar el backend, es necesario crear la base de datos PostgreSQL con el nombre `parcial_catalogo`.

Por ejemplo, desde psql:

```sql
CREATE DATABASE parcial_catalogo;
```


## Backend

### Requisitos
- Python 3.10 o superior
- PostgreSQL

### Instalación
```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

### Configuración
Crear un archivo `.env` dentro de `backend/` con una estructura como esta:

```env
APP_NAME=Parcial Integrador Catálogo
DATABASE_URL=postgresql+psycopg://postgres:TU_PASSWORD@localhost:5432/parcial_catalogo
BACKEND_CORS_ORIGINS=http://localhost:5173,http://127.0.0.1:5173
SQL_ECHO=false
```

### Ejecución
```bash
uvicorn app.main:app --reload
```

Backend disponible en:
- http://127.0.0.1:8000
- http://127.0.0.1:8000/docs

# Frontend

#### Requisitos
- Node.js

#### Instalación
```bash
cd frontend
npm install
```

#### Ejecución
```bash
npm run dev
```

Frontend disponible en:
- http://localhost:5173




