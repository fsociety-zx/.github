# Cómo trabajamos en Kuenta

## Flujo
1. Toma un issue del tablero y muévelo a "In progress".
2. Crea una rama desde `develop` con el ID del issue: `feat/API-11-login-google`, `fix/MOB-31-monto-vacio`.
3. Abre un Pull Request hacia `develop` y escribe `Closes #número`.
4. Con el CI en verde, haz merge con **Squash and merge**.

## Releases
- `main` es producción: solo recibe PRs desde `develop` (o hotfixes).
- PR `develop` → `main` con título "Release vX.Y.Z", usando **Create a merge commit** (nunca squash).
- Después del merge, crea el tag y la release en `main` (Releases → Draft a new release).

## Hotfix
1. Rama desde `main`: `hotfix/descripcion`.
2. PR hacia `main` (merge commit) y release con versión de parche (v1.0.1).
3. PR de `main` → `develop` para no perder el arreglo.
4. 
