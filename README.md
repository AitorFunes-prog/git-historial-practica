# Práctica 3: Viajando en el Tiempo y Corrigiendo el Historial / Aitor Funes del Pino.

## Respuestas a los Ejercicios de Autoevaluación

**1. Identificación de Versiones:**
El hash abreviado del commit donde solo existía la función sumar (C1) es `90f486d`.

**2. Referencia a un Ancestro:**
El comando exacto para hacer un viaje en el tiempo en modo desacoplado al commit inmediatamente anterior a la etiqueta `v1.0-estable` es:
`git switch --detach v1.0-estable~1`.

**3. Seguridad y Borrado:**
Si hubiera usado `git reset --hard` en lugar de `git revert`, habría borrado los commits del historial. En GitHub, esto provocaría que mi historial público difiera del historial local de mis compañeros, causando errores de sincronización y conflictos de fusión graves. `git revert` es seguro porque deshace los cambios añadiendo un nuevo commit, avanzando el historial en lugar de destruirlo.

**4. Propósito de HEAD:**
Tras aplicar el `amend`, HEAD está apuntando a la rama principal, lo cual se comprueba al ver `(HEAD -> main)` en el registro. No me encuentro en un estado de "Detached HEAD".
