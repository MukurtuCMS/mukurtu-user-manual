# Project overview

This repo is the **Mukurtu 4 User Manual**, the end-user documentation site for Mukurtu CMS. It's a content repo, not a codebase: the primary "source" is Markdown articles, and the main job here is writing and organizing documentation, not writing code.

- Built with [MkDocs](https://www.mkdocs.org/) + the [Material](https://squidfunk.github.io/mkdocs-material/) theme.
- Published via Read the Docs (`.readthedocs.yml`, Python 3.12).

# Local build and preview

A `venv/` already exists in the repo root.

```
source venv/bin/activate
pip install -r requirements.txt   # only if deps have drifted
mkdocs serve                      # local preview at http://127.0.0.1:8000
mkdocs build                      # full static build, outputs to site/
```

# Repo layout

- `docs/<topic-folder>/` — article content, one subfolder per topic (e.g. `collections/`, `media/`, `local-contexts/`).
- `docs/_embeds/` — all screenshot/image files referenced by articles.
- `docs/styleguide.md` — the authoritative, detailed content/formatting style guide. Read it before making non-trivial content changes; this file only summarizes it.
- `mkdocs.yml` — site config. **Only edit the trailing `nav:` block.** Do not change plugins, theme, or markdown_extensions config without being asked.

## Do not edit

Per `docs/styleguide.md`, these are out of scope for content work:

- `docs/_static/` (theme assets)
- `requirements.txt`
- `site/` and `venv/` (build output / virtualenv)
- `.gitattributes`, `.gitignore`, `.readthedocs.yml`, `README.md`
- Anything in `mkdocs.yml` outside the `nav:` block

# Content and style rules (summary — see `docs/styleguide.md` for full detail)

- **Folder names**: lowercase, hyphen-separated (e.g. `digital-heritage-items`).
- **Article filenames**: CamelCase, no separators, end in `.md` (e.g. `CreateCollection.md`).
- **Navigation**: an article must be added to the `nav:` block in `mkdocs.yml` to appear on the site — MkDocs will build it without a warning-free build if you skip this, but it won't be reachable from the site nav.
- **Titles/headings**: H1 title in title case with a blank line after; H2-H4 section headings in sentence case, blank line after.
- **Front matter**: optional meta tags before the title, e.g. `pdf: false`, `tags: [...]` — tag values must come from the fixed list in the style guide.
- **Links**: internal links are relative paths without the `.md` extension; external links get `{target=_blank}`.
- **Images**: place files in `docs/_embeds/`, lowercase hyphenated filenames, always include alt text, place images below their corresponding text.
- **Formatting conventions**: buttons in quotes (`"save"`), interface features in **bold**, field names in *italics*, code/paths/URLs in `code formatting`. Mukurtu terms (community, cultural protocol, digital heritage item) stay lowercase unless a proper noun.
- **Tone**: plain language, concise, active voice (passive for warnings/errors), "select" instead of "click", descriptive link text, no ableist language. Writing should work for a wide range of technical skill levels and an international audience.

# Workflow

- Feature branches are short and topic-named (e.g. `collections`, `taxonomies-topic`), merged to `main` via PR.
- No CI runs on this repo currently — verify content changes by running `mkdocs serve` and checking the page locally.
