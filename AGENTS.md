# AGENTS.md
Contexto del proyecto para los agentes de IA. Léalo antes de cualquier cambio.
## Proyecto
Plataforma web lúdica de cursos para niños.
- Curso: Matemáticas | Mecánica: Estrellas
- Roles: docente y niño. El niño entra con código de clase y avatar, sin correo.
## Stack
- Python 3.11+, FastAPI, Jinja2
- SQLModel (SQLite dev / PostgreSQL prod)
- pytest con TestClient, Ruff
- GitHub Actions (CI), Render (despliegue)
## Comandos
- Instalar: `pip install -r requirements-dev.txt`
- Ejecutar: `uvicorn app.main:app --reload`
- Pruebas: `pytest -v`
- Estilo: `ruff check .`
## Estructura
- `app/rutas/`: peticiones → servicios; sin regla de negocio
- `app/servicios/`: regla de negocio y pruebas propias
- `app/modelos/`: tablas SQLModel
- `app/templates/` y `app/static/`: interfaz y PWA
- `tests/`: pruebas; `tests/aceptacion/`: criterios de la especificación
## Convenciones
- Nombres en español, claros y completos.
- Cambios pequeños, una tarea por rama, prueba antes del código.
## Qué no hacer
- No escribir claves ni contraseñas en el código: variables de entorno.
- No instalar dependencias sin verificar que existen en pypi.org.
- No modificar ni borrar pruebas para que pasen.
- No usar datos personales reales.
- No hacer commit ni push: los hace el
desarrollador.
- Al iniciar cada sesión, leer STATE.md.
## Lecciones aprendidas
Registre aquí reglas para no repetir errores.
