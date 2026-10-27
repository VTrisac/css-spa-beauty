# GlowQueen · CSS Proyecto 1 (Spa & Beauty)

Maquetación del diseño 1 de la relación de proyectos de CSS: el hero de *GlowQueen* (spa y belleza), fiel al Figma en escritorio (1920px) y adaptado a portátil, tablet y móvil.

## Qué incluye
- Cabecera con logo, menú y botones de búsqueda y carrito.
- Hero dividido: texto, botones y estadísticas a la izquierda; foto de la modelo con las citas flotantes a la derecha sobre los bloques de color.
- Estados `:hover` y `:focus-visible` en enlaces y botones.
- Responsive con breakpoints en 1500, 1100, 860 y 520px, sin scroll horizontal.

## Estructura
```
index.html
scss/   _fonts, _variables, _base, _components, _layout, _responsive, styles.scss
css/styles.css   (compilado)
assets/img, assets/fonts
```

## Sass
Los estilos se escriben en `scss/` (parciales para variables, base, componentes, layout y responsive) y se compilan a `css/styles.css`, que es el que enlaza el HTML. El CSS compilado ya va incluido, así que la web funciona tal cual. Para recompilar:
```bash
npx sass scss/styles.scss css/styles.css          # una vez
npx sass --watch scss/styles.scss css/styles.css  # mientras editas
```
(o la extensión *Live Sass Compiler* de VS Code).

## Fuentes
Alojadas en `assets/fonts/` (woff2, subconjunto latino) y cargadas con `@font-face`, sin depender de Google Fonts.

## Ver en local
Basta con abrir `index.html` en el navegador o usar Live Server.

## Publicar en GitHub Pages
1. Crea un repositorio público y sube el contenido de esta carpeta a la rama `main`.
2. Settings → Pages → *Deploy from a branch* → `main` / `(root)` → Save.
3. En un minuto estará en `https://<tu-usuario>.github.io/<repositorio>/`. Ese enlace es el que se entrega.
