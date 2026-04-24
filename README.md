# Data Science Unit Site

This repository contains a small MkDocs site for the Data Science Unit using the Material theme.

## Structure

- `mkdocs.yml`: site configuration
- `content/`: markdown source files

## Pages Setup

This project is configured so that MkDocs reads from `content/` and writes the generated site into `docs/`.
GitHub Pages is deployed by the workflow in `.github/workflows/pages.yml`.


## Local Build

Install the dependencies and build the site:

```bash
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install .
mkdocs build --strict
```

## Content Pages

- `content/index.md`
- `content/whatwedo.md`
- `content/principles.md`
- `content/showroom.md`
- `content/contact.md`
