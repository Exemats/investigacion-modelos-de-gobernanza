# Modelos de Gobernanza de Derechos Humanos en Entornos Digitales

Sitio de documentación con el **Estudio Regional sobre Modelos de Gobernanza de Derechos Humanos en Entornos Digitales**, investigación de Civic House en el marco del proyecto de la Fundación Dignitas por la Vida, con el apoyo de AECID.

El contenido original (Google Docs → Markdown) se dividió en capítulos navegables y se publica como un sitio estático con [Jekyll](https://jekyllrb.com/) y el tema [Just the Docs](https://just-the-docs.com/) (barra lateral, búsqueda y navegación por breadcrumbs, en un flujo similar a GitBook).

## Estructura del contenido

- `index.md` — inicio
- `introduccion.md`, `estado-del-arte.md`, `marco-teorico.md`, `metodologia.md`
- `analisis-regulatorio/` — marco global/regional y panorama regional comparado
- `paises/` — nueve fichas nacionales (Argentina, Colombia, Chile, Costa Rica, Panamá, Perú, México, Guatemala, República Dominicana)
- `tendencias-regionales.md`, `conclusiones.md`, `recomendaciones.md`
- `entrevistas/` — Carolina Botero, Cristian León
- `referencias.md`

## Publicar el sitio en GitHub Pages

**Importante:** este repo trae un único workflow (`.github/workflows/pages.yml`). Si en algún momento usás el asistente de GitHub ("Settings → Pages → configurar Jekyll automáticamente"), **no lo aceptes** — crea un segundo workflow (`jekyll.yml`) que duplica y rompe el despliegue.

1. Ir a **Settings → Pages** y en **Build and deployment → Source** elegir **GitHub Actions** (sin usar ningún asistente/plantilla sugerida).
2. Al hacer push a `main`, el workflow existente compila el sitio con Jekyll y lo despliega automáticamente.
3. La URL pública queda disponible en la misma sección de Settings → Pages una vez completado el primer deploy (podés verificar el progreso en la pestaña **Actions**).

## Desarrollo local

```bash
bundle install
bundle exec jekyll serve
```

Sitio disponible en `http://127.0.0.1:4000`.
