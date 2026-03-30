# Data Science Unit Site

This repository contains a small MkDocs site for the Data Science Unit using the Material theme.

## Structure

- `mkdocs.yml`: site configuration
- `content/`: markdown source files
- `docs/`: built static site output for GitHub Pages

## Pages Setup

This project is configured so that MkDocs reads from `content/` and writes the generated site into `docs/`.
That works well when GitHub Pages is configured to publish from the `main` branch and the `/docs` folder.

## Local Build

Install the dependencies and build the site:

```bash
python3 -m venv .venv
.venv/bin/pip install .
.venv/bin/mkdocs build
```

Then commit the generated files in `docs/` so GitHub Pages can serve them.

If you prefer, `requirements.txt` is also included for a lightweight install path.

## Content Pages

- `content/index.md`
- `content/showroom.md`
- `content/contact.md`
