# AI Hero – AI Agents Crash Course

Todo mi trabajo del curso en un solo repo: los ejercicios guiados y mi proyecto personal.

## Índice

- [1. Course – ejercicios del curso](#1-course--ejercicios-del-curso)
- [2. Project – mi proyecto personal](#2-project--mi-proyecto-personal)
- [Cómo correrlo](#cómo-correrlo)

---

## 1. Course – ejercicios del curso

Carpeta: [`course/`](course/)

Ejercicios guiados de cada día. Se trabaja con los repos de ejemplo del curso.

| Día | Notebook | Qué se hace |
|-----|----------|-------------|
| 1 | [`day1.ipynb`](course/day1.ipynb) | Descargar repos de GitHub como zip, parsear los `.md`/`.mdx` con `python-frontmatter` y armar `read_repo_data(owner, repo)` |

**Datos usados:** [`DataTalksClub/faq`](https://github.com/DataTalksClub/faq) y [`evidentlyai/docs`](https://github.com/evidentlyai/docs).

**Dependencias:** `requests`, `python-frontmatter` (dev: `jupyter`).

---

## 2. Project – mi proyecto personal

Carpeta: [`project/`](project/)

Mi propio agente conversacional, construido día a día sobre un repo de documentación que elegí.

**Repo elegido:** [`modelcontextprotocol/modelcontextprotocol`](https://github.com/modelcontextprotocol/modelcontextprotocol)

| Día | Notebook | Qué se hace |
|-----|----------|-------------|
| 1 | [`project1.ipynb`](project/project1.ipynb) | Ingesta de datos: descarga del repo, parseo de markdown y frontmatter, inspección |

### Día 1 – Ingesta

Resultado de la inspección:

- **Documentos:** 451 (363 `.mdx` y 88 `.md`)
- **Con frontmatter:** 392
- **Campos más comunes:** `title` (390), `description` (202), `sidebarTitle` (87)
- **Otros campos:** `date`, `tags`, `author`, `type`, `publishDate`, `weight`, `slug`, `draft`, entre otros

**Dependencias:** `requests`, `python-frontmatter` (dev: `jupyter`).

---

## Cómo correrlo

Cada carpeta es un proyecto `uv` independiente:

```bash
cd course    # o: cd project
uv sync
uv run jupyter notebook
```
