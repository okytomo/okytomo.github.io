# Okytomo — web portfolio

Sitio estático (HTML + CSS, sin build) del portfolio de artista de Okytomo (Octavio Castiñeira), rearmado desde su ex Adobe Portfolio.

## Estructura
- `site/index.html` — la web completa (una sola página: Artworks, Exhibitions, About, Contact).
- `site/img/` — imágenes optimizadas para web (máx 1800px, JPG q82; GIFs originales).
- Cada `article.work` se pliega por JS (script al final de `index.html`): muestra título, texto recortado, tira de miniaturas y botón "View all N …". Para sumar un proyecto nuevo basta copiar la estructura de un `article.work` existente; el plegado se arma solo.
- Bilingüe EN/ES: cada texto va dos veces, `lang="en"` y `lang="es"` (párrafos sueltos, o un `<div lang>` por idioma en el texto de cada proyecto); el CSS oculta el idioma inactivo según `html[data-lang]`. Los títulos de obras y capítulos NO se traducen. Al sumar contenido, cargar siempre los dos idiomas.
- `site/video/` — los 25 videos recuperados de Adobe (Ruins, Enigmatic Events, EWL [The Prequel], Virtual Landscapes, capítulos de Enjoy What's Left, CAOS, No existe tierra más allá). Posters web en `site/img/p_<nombre>.jpg`.
- `originales/` — imágenes tal como se bajaron de Adobe Portfolio, por proyecto; `originales/videos-posters/` tiene los stills de video a resolución completa.
- `.claude/serve.ps1` — servidor estático local (http://localhost:8080) para previsualizar; no hay Python/Node en esta máquina.

## Deploy
GitHub Pages: https://okytomo.github.io (repo público `okytomo/okytomo.github.io`). Cada push a `main` publica la carpeta `site/` vía `.github/workflows/pages.yml` (Pages en modo "GitHub Actions", no "deploy from branch"). `originales/` está en `.gitignore`: queda solo en local. Límite de GitHub: 100 MB por archivo (el video más grande pesa ~48 MB).

## Pendientes
- Sin video recuperado (quedaron fuera de la web): "Mar rojo", "La voz del viento" (Virtual Landscapes) y "Pursuit" (Ruins).
- Sumar proyectos recientes (Sol Negro, fotogrametría, instalación).

## Estilo
Oscuro (ash #0c0d0f, bone #e6e1d6, lunar #86b0cf). Fuentes: Michroma (display), Newsreader (texto), IBM Plex Mono (datos).
