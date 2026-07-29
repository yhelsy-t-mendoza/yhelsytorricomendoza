# Portafolio — Yhelsy Torrico Mendoza

Sitio web multipágina, estático (solo HTML + CSS + JS, sin frameworks ni proceso de build), listo para GitHub Pages.

## Estructura

```
index.html          → Inicio
about.html           → Sobre mí (educación, idiomas, certificaciones)
research.html        → Papers e investigaciones
experience.html       → Prácticas y experiencia profesional/institucional
organizations.html    → Organizaciones fundadas y roles de liderazgo
awards.html            → Becas, premios y reconocimientos
contact.html           → Contacto y descarga de CV
css/styles.css         → Todo el diseño (paleta, tipografía, layout)
js/main.js             → Menú móvil + animación sutil al hacer scroll
```

## Cómo publicarlo en GitHub Pages (paso a paso)

1. Crea un repositorio nuevo en GitHub, por ejemplo `yhelsy-portfolio`.
2. Sube **todos** estos archivos y carpetas a la raíz del repositorio (arrastra y suelta en la web de GitHub, o usa `git add . && git commit -m "sitio inicial" && git push`).
3. En el repositorio, ve a **Settings → Pages**.
4. En "Build and deployment", elige **Deploy from a branch**, rama `main`, carpeta `/root`.
5. Guarda. En 1–2 minutos tu sitio estará en `https://tu-usuario.github.io/yhelsy-portfolio/`.
6. Si quieres un dominio como `yhelsytorrico.com`, cómpralo y configúralo en la misma sección de Pages ("Custom domain").

## Cómo editar contenido (sabiendo solo HTML)

Cada página es HTML plano — puedes editar el texto directamente entre las etiquetas. Ejemplos:

- Para cambiar un título: busca `<h3>...</h3>` y reemplaza el texto.
- Para agregar un premio nuevo: copia un bloque `<div class="award">...</div>` completo dentro de `awards.html` y cambia los textos.
- Para agregar un paper nuevo: copia un bloque `<div class="paper">...</div>` en `research.html`.
- Para agregar una organización o experiencia: copia un bloque `<article class="card">...</article>`.

No necesitas tocar `css/styles.css` para agregar contenido — solo copia y pega los bloques existentes.

## Para subir tu CV y papers en PDF

1. Crea una carpeta `cv/` en el repositorio y sube tu CV con el nombre `Yhelsy_Torrico_Mendoza_CV.pdf` (el botón en `contact.html` ya apunta ahí).
2. Crea una carpeta `papers/` para tus PDFs de investigación y actualiza los enlaces `href="#"` en `research.html` por, por ejemplo, `href="papers/genero-cuotas-bolivia.pdf"`.

## Sistema de diseño ("Case File")

El concepto visual trata cada sección del sitio como un **case file / dossier oficial** — inspirado en tu propio mundo (tribunal electoral, MUN, resoluciones municipales), no en una plantilla genérica.

- **Colores**: tinta casi-negra con base violeta (`#241428`), papel blanco con un tinte lavanda muy sutil (`#FBF9FC`), magenta-ciruela vívido (`#93195E`) como acento principal — una referencia a los colores históricos del movimiento sufragista (violeta + dorado), reinterpretados para verse profesionales e internacionales — y dorado (`#B7893A`) para honores.
- **Tipografía**: Fraunces en pesos altos (600–800, para títulos con más presencia y "llamativos"), Space Grotesk (texto, con más carácter que una sans genérica), IBM Plex Mono (números de expediente, fechas, metadatos).
- **Elemento distintivo**: el sello circular ("YTM") en cada membrete, y la numeración tipo "Case File No. 00X" en cada página.

Para cambiar colores, edita solo las variables al inicio de `css/styles.css` (bloque `:root`) — todo el sitio se actualiza automáticamente.

## Nota sobre el idioma

El sitio está ahora **en inglés**, como versión principal — pensado para que sea la que muestres en tus postulaciones a universidades e internships internacionales, que son mayormente en inglés. Si necesitas una versión en español para becas específicas, lo más simple (sabiendo solo HTML) es crear una carpeta `/es/` con copias traducidas de estas mismas páginas, y agregar un enlace "ES" en el membrete de cada página que apunte a su versión en español. Pídemelo cuando quieras y te la preparo.
