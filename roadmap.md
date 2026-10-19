# Roadmap · Posicionamiento web (SEO)

Plan de trabajo para mejorar el posicionamiento de maarstudiocreativo.com.

## Punto de partida

Medición en Google PageSpeed Insights (19/10/2026):

| Métrica | Móvil | Ordenador | Objetivo |
|---|---|---|---|
| Rendimiento | 85 | 75 | 90+ |
| Carga del contenido principal (LCP) | 3,8 s | 9,0 s | < 2,5 s |
| Peso de la página | 114 MB | 114 MB | < 5 MB |
| SEO | 91 | 91 | 100 |
| Accesibilidad | 92 | 92 | 95+ |

---

## Opción A · Esencial

### Rendimiento (PageSpeed Insights)

- [ ] Convertir las imágenes del portfolio (`assets/proyectos/portfolio/`) a WebP/AVIF en varios tamaños con `srcset` y `sizes`
- [ ] Optimizar las imágenes de fondo (`assets/portatil.jpeg`, `assets/image00002.jpeg`) y la de Nosotros (`assets/image00001.jpeg`)
- [ ] Redimensionar los logos (`assets/4.png`, `assets/5.png`) al tamaño real de uso
- [ ] Añadir `loading="lazy"` y `decoding="async"` a las imágenes que no aparecen en la primera pantalla
- [ ] Añadir `width` y `height` explícitos a todas las imágenes
- [ ] Optimizar la carga de fuentes: quitar las familias sin uso (Raleway, Montserrat, Open Sans Condensed) y evitar que bloqueen el renderizado
- [ ] Minificar el CSS
- [ ] Añadir `vercel.json` con caché de larga duración para `/assets`

### Indexación

- [ ] Crear `robots.txt`
- [ ] Crear `sitemap.xml`
- [ ] Añadir URL canónica
- [ ] Redirigir `/index.html` a `/` y cambiar el enlace del logo a `/`
- [ ] Crear página `404.html`
- [x] Retirar del despliegue los archivos que la web no usa (`.vercelignore`)

### Metadatos y datos estructurados

- [ ] Título orientado a búsquedas (servicio + ubicación)
- [ ] Meta description
- [ ] Open Graph y Twitter Card con imagen para compartir
- [ ] Set de favicons (32 px, 180 px apple-touch, 192/512 px + `site.webmanifest`)
- [ ] JSON-LD `ProfessionalService` (zona de servicio Mallorca, servicios, redes en `sameAs`)
- [ ] JSON-LD `Person` (Mar Fàbregas, fundadora)

### Versión en inglés indexable

- [ ] Generar `/en/` como página estática con los textos de `translations.js`
- [ ] Etiquetas `hreflang` (`es`, `en`, `x-default`) en ambas versiones
- [ ] El selector de idioma enlaza a la URL de cada idioma
- [ ] Añadir `/en/` al sitemap

### SEO on-page y semántica

- [ ] H1 y H2 con palabras clave y ubicación
- [ ] Categorías de proyectos (Restauración, Golf, Moda) como encabezados y orden correcto de encabezados
- [ ] Textos alternativos descriptivos en todas las imágenes
- [ ] Ubicación y datos de contacto visibles en el footer
- [ ] Envolver el contenido principal en `<main>`
- [ ] Menú hamburguesa como `<button>` accesible
- [ ] Corregir contraste del botón principal y otros elementos señalados por PageSpeed
- [ ] Año dinámico en el copyright

### Analítica y medición

- [ ] Google Analytics 4 con Consent Mode v2
- [ ] Banner de cookies acorde con `politica-cookies.html`
- [ ] Verificación en Google Search Console

### Alta en buscadores

- [ ] Configurar `www` en DNS (CNAME a Vercel) y redirigir a la versión sin `www`
- [ ] Alta en Google Search Console y envío del sitemap
- [ ] Alta en Bing Webmaster Tools y envío del sitemap
- [ ] Apoyo en la creación del perfil de Google Business

### Visibilidad en asistentes de IA

- [ ] Crear `llms.txt` con resumen de la web (servicios, proyectos y contacto)

### Cierre

- [ ] Nueva medición en PageSpeed Insights (móvil y ordenador) y comparación con el punto de partida
- [ ] Revisar que no haya errores en Search Console tras la indexación

---

## Opción B · Completo

Incluye todo lo de la Opción A, más lo siguiente.

### Textos (aportados por Mar)

- [ ] Recibir textos de las 4 páginas de servicio
- [ ] Recibir textos de los 7 casos de estudio

### Páginas de servicio

- [ ] `/servicios/estrategia/`
- [ ] `/servicios/diseno-y-branding/`
- [ ] `/servicios/creacion-de-contenido/`
- [ ] `/servicios/gestion-de-redes-sociales/`
- [ ] Cada página con título, meta description, H1, llamada a contacto y JSON-LD `Service`
- [ ] Enlazar las tarjetas de servicios de la home a su página
- [ ] Añadir las páginas al sitemap

### Casos de estudio

- [ ] `/proyectos/mallorca-restaurant-week/`
- [ ] `/proyectos/izakaya/`
- [ ] `/proyectos/captain-hook/`
- [ ] `/proyectos/burc/`
- [ ] `/proyectos/nou/`
- [ ] `/proyectos/the-battle-of-stars/`
- [ ] `/proyectos/sa-roqueta/`
- [ ] Cada página con galería optimizada, título y meta description
- [ ] Enlazar cada proyecto desde la sección Proyectos de la home
- [ ] Añadir las páginas al sitemap

### Sesión de formación

- [ ] Sesión de 1 h: optimizar el perfil de Google Business, conseguir reseñas y darse de alta en directorios
