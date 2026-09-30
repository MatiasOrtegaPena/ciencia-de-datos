# Bitácora de progreso

## Semana 1 — 2026-09-30
- Fase actual: Fase 0 (casi cerrada) → empezando Fase 1
- Lo que terminé:
  - Estructura de carpetas del plan y repo `ciencia-de-datos` publicado en GitHub
  - Git configurado y llave SSH conectada
  - Entorno `ds-signed` funcionando en VS Code
  - Notebook `00-setup/hola_mundo.ipynb` con "Hola mundo" y un gráfico
- Lo que me costó:
  - El kernel del entorno `ds` dejó de arrancar (`spawn UNKNOWN`). Causa: Smart App Control de Windows bloqueaba su `python.exe` por no estar firmado. Lo diagnostiqué con el log de Code Integrity y lo resolví creando un entorno nuevo con el canal `defaults` de Anaconda (firmado).
  - Guardar el notebook antes de hacer commit: subí una versión vacía porque no había guardado (`Ctrl + S`). Lección: `git status` y `git diff` antes de `git add`.
  - Usar `git commit -m` (no `-n`, que es `--no-verify`).
- Commits / repos actualizados: `ciencia-de-datos` (7 commits + los de esta actualización)
- Próxima semana:
  - Empezar CS50P (Fase 1)
  - Missing Semester: clases 1 (shell) y 6 (Git)
  - Etiquetas con unidades en el gráfico del notebook
  - Borrar el entorno `ds` cuando el otro proyecto use `ds-signed`
  - Mini examen de la Fase 0
