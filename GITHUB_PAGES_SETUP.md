# Cómo se publica esta web

GitHub Pages está configurado para **servir directamente desde la rama `main`**.
Cada push despliega: lo hace el constructor nativo de GitHub, el que aparece en
Actions como «pages build and deployment».

No hay que hacer nada más.

## Por qué ya no hay workflow propio

Había un `.github/workflows/pages.yml` que usaba `peaceiris/actions-gh-pages`.
Fallaba en cada push y no desplegaba nada: le faltaban permisos de escritura
(`permissions: contents: write`), que GitHub dejó de conceder por defecto a
`GITHUB_TOKEN` después de que se escribiera ese fichero.

Como quien publica de verdad es el constructor nativo, el workflow solo servía
para mandar un correo de fallo en cada push. Se eliminó el 12 de noviembre
de 2026.

Si algún día hace falta un paso de compilación —no lo hace: son ficheros HTML
sueltos— habría que recuperarlo con los permisos correctos y cambiar Pages a
«GitHub Actions» como origen.

## Qué hay publicado

| Fichero | URL |
|---|---|
| `index.html` | https://josefranruiz.github.io/madrid-parks-landing/ |
| `index-es.html` | …/index-es.html |
| `privacy.html` | …/privacy.html |
| `status.html` | …/status.html |

`privacy.html` es la dirección registrada en App Store Connect. **No se renombra
ni se mueve.**
