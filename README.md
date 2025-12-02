# RRIMPORT Catálogo (GitHub Pages)

Sitio estático con React (CDN) y Tailwind para mostrar el catálogo de carrocería e iluminación de RRIMPORT (Hilux 2021-2023). Se ejecuta directo desde `/public` sin build, listo para publicarse en GitHub Pages.

> Nota: existe un `index.html` en la raíz que redirige automáticamente a `public/` para que la página cargue aun si Pages está configurado a publicar desde la rama principal sin workflow.

## Cómo publicar en GitHub Pages
1. Habilita **Pages** en la configuración del repositorio y selecciona "GitHub Actions" como fuente.
2. El workflow `.github/workflows/deploy.yml` publicará automáticamente el contenido de `public/` en cada push a la rama principal.
3. La URL final seguirá el patrón `https://<usuario>.github.io/CatalogsRR/`.

## Desarrollo y vista previa local
No se necesitan dependencias adicionales. Para un servidor local rápido ejecuta:

```bash
python -m http.server 4173 -d public
```

Luego abre [http://localhost:4173](http://localhost:4173) en tu navegador.
