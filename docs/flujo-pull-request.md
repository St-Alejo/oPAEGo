# Flujo de trabajo con pull requests

1. Crear una rama desde `main` con prefijo según el cambio: `feat/`, `fix/`, `docs/`, `ci/`.
2. Commits en Conventional Commits en español: `tipo(ámbito): resumen en imperativo`.
3. Abrir el pull request hacia `main`. Si aún no está listo, abrirlo como **borrador**.
4. El compañero revisa: el CI (estilo, pruebas y cobertura) debe quedar en verde.
5. Fusionar y borrar la rama.

Cada paso queda registrado en monday: el PR aparece en el sprint que corresponde y
su estado cambia solo (En curso → En revisión → Hecho).
