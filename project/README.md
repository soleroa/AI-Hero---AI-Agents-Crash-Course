# Project – mi proyecto personal

Agente conversacional sobre la documentación de [`modelcontextprotocol/modelcontextprotocol`](https://github.com/modelcontextprotocol/modelcontextprotocol), construido día a día. Parte del [índice general](../README.md).

## Contenido

| Día | Notebook | Qué se hace |
|-----|----------|-------------|
| 1 | [`project1.ipynb`](project1.ipynb) | Ingesta: descarga del repo, parseo de markdown y frontmatter, inspección |

## Día 1 – Ingesta

- **Documentos:** 451 (363 `.mdx` y 88 `.md`)
- **Con frontmatter:** 392
- **Campos más comunes:** `title` (390), `description` (202), `sidebarTitle` (87)
- **Otros campos:** `date`, `tags`, `author`, `type`, `publishDate`, `weight`, `slug`, `draft`, entre otros

## Cómo correrlo

```bash
uv sync
uv run jupyter notebook
```
