# Fase 0 — Instalación y herramientas

**Objetivo:** dejar listo el entorno de trabajo (Git, VS Code, Miniconda, GitHub) y perderle el miedo a la terminal.

## Entregable
- [x] Repo `ciencia-de-datos` en GitHub con `progreso.md`
- [x] Al menos 5 commits
- [x] Entorno `ds-signed` funcionando (ver nota abajo)
- [x] Notebook que imprima "Hola mundo" y un gráfico simple ([hola_mundo.ipynb](hola_mundo.ipynb))

## Pendiente
- [ ] Missing Semester (MIT): clases 1 (shell) y 6 (Git)
- [ ] Etiquetas con magnitud y unidades en los ejes del gráfico

## Nota: por qué el entorno se llama `ds-signed`
El entorno `ds` original (conda-forge) fue bloqueado por **Smart App Control** de Windows, porque su `python.exe` no está firmado digitalmente. El síntoma en VS Code era `Failed to start the Kernel ... spawn UNKNOWN`. La solución fue crear un entorno nuevo con el canal `defaults` de Anaconda, cuyo `python.exe` sí está firmado:

```bash
conda create -n ds-signed python=3.12 --override-channels -c defaults
python -m pip install numpy pandas matplotlib seaborn jupyter scikit-learn
```
