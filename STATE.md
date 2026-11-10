# STATE.md

Estado del proyecto. Léalo al iniciar cada sesión de trabajo y actualícelo al cerrarla.

## Estado actual
Repositorio publicado en GitHub con el CI en verde.
Página de inicio, /salud y /docs funcionando en https://plataforma-ludica-

abcd.onrender.com.
Se agregó GET /api/version, que devuelve la versión configurada en app/proyecto.py.
## Decisiones
| Fecha | Decisión | Motivo |
| --- | --- | --- |
| AAAA-MM-DD | Usar la plantilla del curso con FastAPI | Es el stack definido para el
proyecto |
| 2026-11-10 | Reutilizar proyecto.VERSION en GET /api/version y cubrirlo con una prueba | Mantener una fuente única para la versión y verificar el endpoint |
## Siguiente paso
Ejecutar la prueba de tests/test_inicio.py cuando el entorno tenga disponibles las dependencias necesarias; la ejecución de hoy no pudo recolectar las pruebas porque falta httpx.