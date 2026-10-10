# dantezulli.ar 🇦🇷

Blog personal de Dante Zulli. Hecho con [Hugo](https://gohugo.io/) + tema [Bear Cub](https://github.com/clente/hugo-bearcub).

El contenido vive en Markdown bajo `content/`. Deploy en Cloudflare Pages
desde `public/` (ver `wrangler.jsonc`).

## Comandos

| Comando | Qué hace |
|---|---|
| `hugo server -D` | Servidor local con drafts (http://localhost:1313) |
| `hugo` | Build de producción (genera `public/`) |
| `hugo --printI18nWarnings --printPathWarnings` | Build con advertencias (debug) |

## Posts / Proyectos nuevos

```bash
hugo new content blog/mi-post/index.md
hugo new content proyectos/mi-proyecto/index.md
```

Los posts nuevos arrancan como `draft = true`. Para publicarlos, pasalos a `draft = false`.
Los proyectos pueden tener un `link` en el front matter para redirigir externo.

## Estructura

```
content/
├── _index.md              # Home
├── blog/                  # Posts
├── contacto/              # /contacto/
├── now/                   # /now/
└── proyectos/             # /proyectos/
layouts/                   # HTML templates (Bear Cub copiado acá)
assets/                    # CSS e imágenes
i18n/                      # Traducciones (es.toml)
```

## URLs

`/` · `/blog/` · `/blog/:post/` · `/proyectos/` · `/proyectos/:proyecto/` · `/contacto/` · `/now/` · `/index.xml`

## Performance

Link a [Google PageSpeed Insights](https://pagespeed.web.dev/)

## Deploy (Cloudflare Pages)

- Framework preset: **Hugo**
- Build command: `hugo`
- Output directory: `public`
- Production domain: `https://www.dantezulli.ar`

## License

Contenido del sitio: CC BY 4.0.
Código: MIT (ver [LICENSE](LICENSE)).
