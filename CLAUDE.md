# Okytomo — web portfolio

Sitio estático (HTML + CSS, sin build) del portfolio de artista de Okytomo (Octavio Castiñeira), rearmado desde su ex Adobe Portfolio.

## Estructura
- `site/index.html` — la web completa (una sola página: Artworks, Exhibitions, About, Contact).
- `site/img/` — imágenes optimizadas para web (máx 1800px, JPG q82; GIFs originales).
- `site/video/` — los 25 videos recuperados de Adobe (Ruins, Enigmatic Events, EWL [The Prequel], Virtual Landscapes, capítulos de Enjoy What's Left, CAOS, No existe tierra más allá). Posters web en `site/img/p_<nombre>.jpg`.
- `originales/` — imágenes tal como se bajaron de Adobe Portfolio, por proyecto; `originales/videos-posters/` tiene los stills de video a resolución completa.
- `.claude/serve.ps1` — servidor estático local (http://localhost:8080) para previsualizar; no hay Python/Node en esta máquina.

## Deploy
Gratis en Netlify: arrastrar la carpeta `site/` a app.netlify.com/drop (o conectar el repo con publish dir `site`). Ojo: `site/` pesa ~390 MB por los videos.

## Pendientes
- Sin video recuperado (quedaron fuera de la web): "Mar rojo", "La voz del viento" (Virtual Landscapes) y "Pursuit" (Ruins).
- Sumar proyectos recientes (Sol Negro, fotogrametría, instalación).

## Estilo
Oscuro (ash #0c0d0f, bone #e6e1d6, lunar #86b0cf). Fuentes: Michroma (display), Newsreader (texto), IBM Plex Mono (datos).
