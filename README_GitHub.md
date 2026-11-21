# XR FUSION EDU — versión corregida

## Modelos integrados
La biblioteca detecta automáticamente los archivos `.glb` de la carpeta `models/` (los 5 incluidos) y los muestra en **BIBLIOTECA 3D**. La portada original se conserva.

## Cómo ejecutar
1. Extrae el ZIP completo.
2. Abre la carpeta extraída en GitHub.
3. Ejecuta `index.html` con la extensión **Live Server** (no con doble clic).
4. Pulsa **ENTRAR AL LABORATORIO**. Los modelos aparecen en **BIBLIOTECA 3D** a la izquierda.

No muevas `index.html` fuera de la carpeta ni separes `models/`: las rutas de los modelos son relativas (`./models/nombre.glb`).

## Si algún modelo no aparece
- Abre **◈ DIAGNÓSTICO**: muestra qué archivos se encontraron.
- La carpeta debe llamarse exactamente `models` (minúsculas) y estar junto a `index.html`.
- En GitHub Pages las mayúsculas importan: `Modelo.glb` y `modelo.glb` son archivos distintos.
- Si no se detecta automáticamente, crea `models/models.json` con la lista de nombres:
  `["archivo1.glb", "archivo2.glb"]`
  o añádelos en la constante `EXTRA_MODEL_FILES` dentro de `index.html`.
