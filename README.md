# 🎬 Planificador de clases por proyecto

Aplicación web (HTML + JavaScript, sin servidor) que ayuda a los docentes a planificar proyectos de TBox Academy.

- **Planificación del trimestre:** sube el PDF del proyecto → calendario semanal con evaluaciones sumativas (70 %) y formativas (30 %) sugeridas. Descarga en PDF y PNG.
- **Planificación de la clase del día:** sube el PDF de la actividad de TBox → guía de la clase, rúbrica, evaluación sumativa y formativa. Descarga en PDF y PNG.

Todo se procesa en el navegador del docente: los PDF no se envían a ningún servidor.

## Publicar con GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `planificador-proyectos`).
2. Sube `index.html` y este `README.md`:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Primera versión"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/planificador-proyectos.git
   git push -u origin main
   ```
3. En GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
4. En 1–2 minutos la app estará en `https://TU_USUARIO.github.io/planificador-proyectos/`.

## Notas

- Usa las librerías pdf.js y jsPDF desde `cdnjs.cloudflare.com`; necesita conexión a internet.
- En esta versión el contenido de las planificaciones sale de plantillas base. La redacción con Claude solo funciona dentro de claude.ai.
- Para añadir IA fuera de claude.ai se necesita un pequeño servidor intermedio que guarde la clave de API (nunca la pongas en `index.html`).
