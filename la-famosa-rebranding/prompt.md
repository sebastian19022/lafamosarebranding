# Página web — Caso de estudio "Rebranding La Famosa"

## Contexto y objetivo

Este es un proyecto de **tesis universitaria**: un rebranding de la marca dominicana de alimentos **La Famosa** (parte de Peravia Industrial desde 1963). Necesito una **página web de una sola sección scrolleable (one-page)** que presente el proyecto de rebranding como si fuera un case study, para mostrarla durante la defensa de tesis.

**No tiene que ser "wow" ni sobrediseñada.** Prioriza: verse limpia, profesional, ordenada, fácil de navegar y que comunique bien el trabajo de rebranding. Es más importante que se vea sólida y coherente con la marca que impresionar con efectos. Evita animaciones exageradas o efectos que puedan fallar en una presentación en vivo.

## Stack sugerido

Sitio estático simple: HTML + CSS + JS vanilla (sin build step), para poder abrirlo directo con un servidor local o subirlo a cualquier hosting sin complicaciones. Si prefieres usar Vite/React está bien también, pero no es necesario — prioriza velocidad de entrega y estabilidad sobre sofisticación técnica.

## Assets incluidos (carpeta `assets/`)

Todos los assets fueron extraídos del PDF de rebranding original. Úsalos tal cual (son renders finales del proyecto):

- `assets/logos/logo-wordmark-red.png` — logotipo "La Famosa" en rojo, fondo transparente. Úsalo en el header/navbar sobre fondos claros.
- `assets/logos/logo-full-tricolor.png` — logo completo con mapa de RD, pluma verde y tagline "LO MÁS NATURAL", fondo transparente. Ideal para el hero.
- `assets/logos/monogram-F.png` — monograma "F" rojo, fondo transparente. Úsalo como favicon o como elemento decorativo pequeño.
- `assets/logos/logo-on-gold.png`, `logo-on-red.png`, `logo-on-navy.png` — lockups del logo sobre los colores de marca (fondo sólido incluido).
- `assets/logos/logo-variations-sheet.png` — hoja completa de variaciones del logotipo (imagen de referencia para una sección "Sistema de marca" si quieres mostrar todas las variantes juntas).
- `assets/productos/familia-productos.png` — línea completa de productos (catchup, aceite de oliva, enlatados) con vegetales frescos, fondo blanco.
- `assets/productos/enlatados-detalle.png` — detalle de 3 latas (vainitas/habichuelas verdes, pasta de tomate, maíz dulce) con vegetales.
- `assets/productos/jugos-horizontal.png` — línea de jugos (pera, piña, fresa) en formato horizontal, fondo dorado.
- `assets/productos/jugos-poster-vertical-1.png` y `jugos-poster-vertical-2.png` — posters verticales de la línea de jugos con el logo, fondo dorado (dos variantes/crops, usa la que mejor encaje).
- `assets/aplicaciones/merchandising-textil.png` — mockups de delantal, gorra, tote bag y carnet/lanyard con el logo aplicado.
- `assets/aplicaciones/camion-carnet-polo-valla.png` — mockups de camión de reparto, carnet corporativo, polo y valla publicitaria (billboard).
- `assets/social/posts-redes-sociales.png` — 3 mockups de posts para redes sociales en formato mobile (con los copies "Sabor que nos une", "La tradición dominicana no se estanca / Evoluciona", "El sabor de nuestra tierra, en tu mesa").

Todas las imágenes ya tienen fondo/composición resuelta (son renders finales de presentación), así que puedes usarlas como imágenes de sección grandes, no necesitas recortarlas más salvo que quieras ajustar el encuadre.

## Contenido de marca (texto real, úsalo tal cual — no inventes copy nuevo salvo llamados a la acción genéricos)

**Nombre de marca:** La Famosa
**Tagline:** "Lo más natural"
**Mensaje de marca (frase ancla):** "La tradición dominicana no se estanca, evoluciona."

**Historia / Nuestra historia:**
> Desde 1963, formando parte de las mesas dominicanas, llevando productos que combinan calidad, tradición y el sabor que nos identifica.
>
> La Famosa inicia su trayectoria como parte de Peravia Industrial, construyendo desde sus primeros años una identidad vinculada a la producción de alimentos y al desarrollo agroindustrial dominicano. A lo largo de las décadas, la marca ha ampliado su presencia y su oferta de productos, manteniendo como parte de su esencia el compromiso con la calidad y las familias dominicanas.
>
> Actualmente, La Famosa cuenta con una amplia variedad de productos destinados al consumo cotidiano, manteniendo su presencia en los hogares dominicanos mientras busca evolucionar junto a las nuevas generaciones.

**Copies de campaña / redes sociales (úsalos en la sección de aplicaciones/social):**
- "Sabor que nos une"
- "La tradición dominicana no se estanca... Evoluciona"
- "El sabor de nuestra tierra, en tu mesa"

**Nuestros productos (categorías):**
- Catchup
- Aceite de Oliva Extra Virgen
- Vegetales enlatados: habichuelas/vainitas verdes, pasta de tomate, maíz dulce, guandules
- Jugos en lata: pera, piña, fresa

## Paleta de colores de marca

Usa estos tonos (aproximados, tómalos de las imágenes si necesitas exactitud de pixel, pero estos valores son un punto de partida fiel):

- **Rojo La Famosa** (color principal del logotipo): `#E4272B` aprox.
- **Azul marino** (texto secundario / "La", tarjetas oscuras): `#1E3A5F` aprox.
- **Dorado/Ámbar** (fondo línea de jugos, acento cálido): `#F2A81D` aprox.
- **Verde** (pluma del logo, acento natural): `#1B7A3D` aprox.
- **Blanco / crema** para fondos limpios y espacio negativo.

## Tipografía

El logotipo usa una **script/cursiva bold** (tipo "brush script", inclinada) para "La Famosa" — no es necesario replicarla exacta en el body text, pero para títulos grandes considera una fuente script similar en Google Fonts (ej. "Pacifico", "Dancing Script" en bold, o "Caveat" bold) SOLO para el nombre de marca o titulares hero, no para texto de lectura. Para el resto del sitio (párrafos, navegación, botones) usa una sans-serif limpia y legible (ej. "Inter", "Poppins" o "Work Sans"), consistente con el tono "LO MÁS NATURAL" — geométrica, cálida, no corporativa-fría.

## Estructura de la página (secciones, en orden)

1. **Header/Nav fijo** — logo pequeño (`logo-wordmark-red.png`) a la izquierda, links de ancla a las secciones (Historia, Marca, Productos, Aplicaciones, Contacto/Cierre) a la derecha. Fondo blanco o crema, sombra sutil al hacer scroll.

2. **Hero** — Fondo dorado o crema. Logo completo grande (`logo-full-tricolor.png`), debajo la frase de marca "La tradición dominicana no se estanca, evoluciona." como titular grande, y un subtítulo corto explicando que es un proyecto de rebranding (ej. "Proyecto de rebranding — [nombre de tesis/universidad si el usuario lo da, si no, dejar un placeholder editable]"). Puedes usar `jugos-poster-vertical-1.png` o `familia-productos.png` como imagen de apoyo lateral.

3. **Nuestra historia** — Layout de dos columnas: texto de la historia (usar el copy real de arriba) a un lado, y una imagen de producto o del logo al otro lado. Línea de tiempo simple opcional (1963 → hoy) si quieres un elemento visual extra, pero no es obligatorio.

4. **Sistema de marca / Identidad visual** — Mostrar el logotipo y sus variantes: usa `logo-on-gold.png`, `logo-on-red.png`, `logo-on-navy.png` en una grilla de 3 tarjetas, y debajo un swatch/paleta de los 4 colores de marca con sus nombres y hex. Opcional: incluir `logo-variations-sheet.png` como imagen completa de referencia.

5. **Nuestros productos** — Mostrar `familia-productos.png` como imagen destacada grande, y debajo una grilla de las categorías de producto (Catchup, Aceite de Oliva, Enlatados, Jugos) cada una con su imagen correspondiente (`enlatados-detalle.png`, `jugos-horizontal.png`) y una descripción corta.

6. **Aplicaciones de marca** — Mostrar `merchandising-textil.png` y `camion-carnet-polo-valla.png` como imágenes grandes (full-bleed o en tarjetas), con un título tipo "La marca en el mundo real" explicando brevemente que el sistema se extiende a uniformes, vehículos de reparto y publicidad exterior.

7. **Campaña / Redes sociales** — Mostrar `posts-redes-sociales.png` junto con los 3 copies de campaña destacados como quotes/citas grandes.

8. **Cierre / Footer** — Logo pequeño, tagline "Lo más natural", y un footer simple (puede incluir un placeholder de "Proyecto académico — [Nombre del autor] — [Año]" editable). No hace falta formulario de contacto real ni links a redes sociales reales — esto es una presentación de tesis, no un sitio de producción.

## Detalles de ejecución

- Responsive: debe verse bien en desktop (para proyectar en la defensa) y razonablemente bien en mobile/tablet, pero el caso de uso principal es pantalla grande/proyector.
- Transiciones/scroll: animaciones suaves y sutiles al entrar cada sección están bien (fade-in / slide-up al hacer scroll), pero nada intrusivo, sin autoplay de video, sin sonido.
- Optimiza las imágenes solo si es trivial (lazy loading con `loading="lazy"` está bien); no hace falta pipeline de compresión.
- Genera un `README.md` corto explicando cómo abrir/servir el sitio localmente (ej. `npx serve` o Live Server).
- Si usas un dev server, verifica que la página cargue y que las imágenes se vean correctamente antes de dar por terminado.

## Lo que NO hacer

- No inventes secciones de e-commerce, carrito de compra, login, ni funcionalidad backend — es una página de presentación estática.
- No reemplaces las imágenes reales por placeholders genéricos de stock; usa los assets provistos.
- No sobrecargues de efectos (parallax pesado, partículas, video hero) — el pedido explícito es que "no tiene que ser wow", solo clara y profesional.
