# La Famosa — Caso de estudio de rebranding

Página web de una sola sección (one-page) para presentar, en formato de caso de estudio, el
proyecto de rebranding de tesis de la marca dominicana **La Famosa**.

Sitio estático: HTML + CSS + JS vanilla, sin build step ni dependencias.

## Cómo verlo localmente

Cualquiera de estas opciones sirve — solo necesitas un servidor local porque el sitio carga
imágenes con rutas relativas.

**Opción 1 — Node (serve):**

```bash
npx serve .
```

**Opción 2 — Python:**

```bash
python -m http.server 5514
```

Luego abre `http://localhost:5514` (o el puerto que indique la terminal).

**Opción 3 — VS Code:** extensión "Live Server", clic derecho sobre `index.html` → *Open with Live Server*.

## Estructura

```
index.html          Marcado y contenido de todas las secciones
css/style.css        Estilos (tokens de color/tipografía, layout, responsive)
js/main.js           Reveal al hacer scroll, header con sombra, menú móvil
assets/               Renders del rebranding (logos, productos, aplicaciones, social)
```

