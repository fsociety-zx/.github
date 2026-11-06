# Cómo trabajamos en Kuenta

## Flujo
1. Toma un issue del tablero y muévelo a "In progress".
2. Crea una rama desde `main` con el ID del issue: `feat/API-11-login-google`, `fix/MOB-31-monto-vacio`.
3. Abre un Pull Request usando la plantilla y escribe `Closes #número` para que el issue se cierre solo.
4. Cuando el CI esté en verde, haz merge con **Squash and merge**.

## Commits (Conventional Commits)
- `feat:` nueva funcionalidad
- `fix:` corrección de error
- `chore:` mantenimiento, configuración
- `docs:` documentación
- `test:` pruebas
- `refactor:` cambio de código sin cambiar comportamiento

Ejemplo: `feat(auth): login con Google`
