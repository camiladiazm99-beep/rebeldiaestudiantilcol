# Mi Blog

Blog de una sola página, autocontenido en un único archivo HTML.

## Cómo usarlo

1. Abre `index.html` en cualquier navegador moderno (Chrome, Safari, Firefox, Edge).
2. Listo — la página funciona sin servidor, sin instalaciones, sin conexión a internet (excepto para cargar las fuentes de Google Fonts la primera vez).

## Cómo subir tu contenido

- **Imagen de portada** — arrastra una imagen (PNG/JPEG/WebP/AVIF) sobre el slot del hero.
- **4 videos verticales** — arrastra un archivo de video sobre cada reproductor, o haz clic para examinar archivos. Formato 9:16 recomendado.
- **Imagen horizontal** — arrastra una imagen sobre el slot grande. Formato 16:9 recomendado.
- **Infografía** — arrastra tu infografía sobre el slot final (formato vertical alto).

Las imágenes se guardan automáticamente. Los videos se cargan localmente desde tu navegador (no persisten al recargar — vuelve a subirlos si refrescas).

Para reencuadrar una imagen ya cargada, **haz doble clic** sobre ella y arrastra.

## Edición de texto

- Haz clic sobre cualquier título editorial, pie de foto o crédito para editarlos directamente (atributo `contenteditable`).
- Los textos del hero (título, subtítulo, fecha, etc.) se editan directamente en el HTML buscando los `id="hero-title"`, `id="hero-lede"`, etc.

## Personalización visual

Si publicas la página en un entorno que soporte el panel Tweaks, podrás cambiar paleta, color de acento, fuente de titulares, densidad y nombre del blog desde la interfaz. Si solo abres el HTML directamente, puedes editar los valores por defecto al inicio del bloque `<script type="text/babel">` que contiene `TWEAK_DEFAULTS`:

```js
const TWEAK_DEFAULTS = {
  "palette": "warm",        // warm, cool, paper, forest, bloom, citrus,
                            // ocean, mono, dark, midnight, espresso, noir
  "accent": "#b8542e",
  "density": "regular",     // dense, regular, airy
  "displayFont": "Instrument Serif",
  "brand": "Mi blog"
};
```

## Publicación

El archivo `index.html` es completamente autónomo. Para publicarlo basta con subirlo a cualquier hosting estático: GitHub Pages, Netlify, Vercel, Cloudflare Pages, un bucket de S3, o el servidor que prefieras.

---

Hecho con ♥
