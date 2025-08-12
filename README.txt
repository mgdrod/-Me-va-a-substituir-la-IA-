
# ¿Me va a sustituir la IA? — Prototipo estático

Este prototipo es una web sencilla que permite buscar una **profesión** y ver:
- **Riesgo de automatización (%)**
- **Tareas susceptibles**
- **Habilidades recomendadas para adaptarse**

## Archivos
- `index.html` — interfaz principal
- `styles.css` — estilos
- `data.json` — base de datos (editable)
- `datos_app_automatizacion.csv` — misma base en CSV para Glide/AppSheet

## Cómo probar en local
1. Descarga los archivos y ábrelos en una carpeta.
2. Haz doble clic en `index.html` (en móvil se recomienda subirlo a GitHub Pages).

## Cómo publicarlo gratis en GitHub Pages
1. Crea un nuevo repositorio en GitHub (público).
2. Sube `index.html`, `styles.css` y `data.json`.
3. En **Settings > Pages**, elige **Deploy from a branch** y selecciona `main` y la carpeta `/root`.
4. Espera 1-2 minutos y entra a la URL que te dará GitHub Pages.

## Cómo llevarlo a Glide (app sin código)
1. Sube `datos_app_automatizacion.csv` a Google Drive y ábrelo con Google Sheets.
2. En **glideapps.com**, crea una app desde Google Sheets.
3. Crea una pantalla con:
   - **Search bar** conectada a la columna `Profesión`
   - **Progress bar** para `Riesgo_Automatizacion_%`
   - **Listas** para `Tareas_Susceptibles` y `Habilidades_Futuras` (puedes dividirlas por coma con Glide)
4. Ajusta los colores según nivel de riesgo (bajo <35, medio <70, alto ≥70).

## Notas metodológicas
- Los porcentajes son estimativos, inspirados en literatura (Oxford, McKinsey, WEF). Ajusta a tu contexto (España) si tienes fuentes específicas.
- Añade más filas o edita `data.json` para ampliar sectores.
- En la presentación, deja claro que es una **herramienta educativa**.

## Ideas de mejora
- Añadir un campo de **salario medio** o **tendencia de demanda**.
- Incluir un **timeline de adopción** por profesión (2025→2035).
- Un botón de **“¿Cómo me preparo?”** con cursos/habilidades recomendadas.
