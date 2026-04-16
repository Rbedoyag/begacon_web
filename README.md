# Begaco — sitio web

Landing estática: una sola página (`index.html`) con estilos y scripts integrados.

Repositorio: [github.com/Rbedoyag/begaco_web](https://github.com/Rbedoyag/begaco_web)

## Publicar con GitHub Pages

1. En GitHub, abre el repositorio **begaco_web**.
2. **Settings** → **Pages** (menú izquierdo).
3. En **Build and deployment** → **Source**: elige **Deploy from a branch**.
4. **Branch**: `main`, carpeta **`/ (root)`** → **Save**.
5. En unos minutos la URL aparecerá arriba (suele ser `https://rbedoyag.github.io/begaco_web/`). La primera carga puede tardar un poco.

No hace falta acción extra en el código: `index.html` en la raíz es suficiente.

## Estructura del repo

| Archivo        | Descripción                          |
|----------------|--------------------------------------|
| `index.html`   | Sitio completo (HTML, CSS, JS).     |
| `.gitignore`   | Excluye carpetas locales (p. ej. `.claude/`). |

## Ideas para mejorar rendimiento y mantenimiento

- **Archivos separados**: extraer CSS y JS a `.css` / `.js` externos mejora la caché del navegador en visitas repetidas.
- **Hero animado**: WebGL + partículas consumen CPU/GPU; conviene reducir o pausar efectos con `prefers-reduced-motion` o equipos modestos.
- **Compartir en redes**: añadir meta etiquetas Open Graph (`og:title`, `og:description`, `og:image`) para previews al pegar el enlace.
- **Enlaces**: sustituir `href="#"` del pie (blog, legales, redes) por URLs reales cuando existan.
