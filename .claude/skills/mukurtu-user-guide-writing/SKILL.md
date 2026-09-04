---
name: mukurtu-user-guide-writing
description: Write or substantially revise a Mukurtu user manual article (informational, instructional, additional, or FAQ) so it follows this repo's file naming, mkdocs.yml nav, front matter, and tone/style conventions. Use for requests like "write a guide for...", "document how to...", "add an article about...", or "update the X article."
---

# Mukurtu User Guide Writing

This repo's authoritative conventions live in `docs/styleguide.md`. **Read that file in full before drafting anything** — it is the source of truth for filenames, tags, admonitions, and tone rules. This skill is the workflow and quick-reference on top of it; where the two disagree, `docs/styleguide.md` wins.

## Workflow

### 1. Scope & placement

Before writing, work out:

- **Article type** (see `docs/styleguide.md` → "Article types and titles"):
  - *Informational* — overview/explanation, named `Understanding ___`, usually the first article under its topic.
  - *Instructional* — how to do something, named `[Verb] [Feature]` (e.g. `Create a Collection`, `Upload a Media Asset`).
  - *Additional* — detailed/technical/reference content, simple free-form title.
  - *FAQ* — question-style title, Q&A body.
- **Topic folder** — an existing folder under `docs/` (hyphenated, lowercase) if the topic already exists; only propose a new folder if nothing fits.
- **User role(s)** involved (site admin, community manager, community member, etc.) — call these out if they affect what the reader can do.
- **Related articles** to link to/from — check `mkdocs.yml`'s `nav` for siblings in the same topic so the new page connects into the existing structure instead of becoming an orphan.

Confirm scope with the user before drafting if the topic folder, article type, or role is ambiguous.

### 2. Draft

- **Filename**: CamelCase, no spaces, omit conjunctions/articles (`CreateCollection.md`, not `CreateACollection.md` — see the style guide's examples for exceptions like `CreateACommunityAndInitialCulturalProtocol.md`).
- **Front matter**: include `pdf: false` if the page shouldn't offer a PDF download, and `tags:` drawn *only* from the approved tag list in `docs/styleguide.md` — never invent a new tag.
- **Title**: H1, title case, one blank line below.
- **Sections**: H2–H4, sentence case, one blank line below each heading.
- **Tone/style** (full rules in the style guide):
  - Active voice, plain language, concise and task-focused.
  - "Select," never "click."
  - Button names in "quotes"; interface features (tabs, page titles, dropdowns) in **bold**; field/label names in *italics*; paths, code, and URLs in `code formatting`.
  - No `-` as a prose separator (fine inside compound words/markdown syntax).
  - Lowercase Mukurtu terms (`community`, `cultural protocol`, `digital heritage item`) except proper nouns like `Mukurtu CMS`, `Local Contexts`.
  - Admonitions (`!!! tip`, `!!! warning`, `!!! requirement`, `!!! roles "User roles"`) need a blank line before and after; the `roles` admonition must keep the "User roles" title override.
- **Screenshots**: place below the text they support (never as a substitute for it), reference via `![Alt text](../docs/_embeds/topic-name-01.png)`, filename lowercase-hyphenated with 2-digit numbering if the article has 10+ images, and always include real alt text.

Use the templates below as a starting skeleton, adapted to the actual feature being documented — don't leave placeholder brackets in the final draft.

#### Informational template

```markdown
# Understanding [Feature]

[One or two sentences: what this is and why it matters to the reader.]

## What is a [feature]?

[Plain-language explanation of the concept.]

## Why use [feature]?

[Task-focused context — when and why a user would do this.]

## Related articles

- [[Verb] [Feature]](VerbFeature)
```

#### Instructional template

```markdown
# [Verb] [Feature]

!!! roles "User roles"
    [Which roles can do this.]

[One-sentence statement of what the reader will accomplish.]

## Prerequisites

- [Anything required before starting, if applicable.]

## Steps to [verb] a [feature]

1. [First step, imperative, one action per step.]
2. [Next step.]
3. Select the "[button]" button.

![Alt text describing the screenshot.](../docs/_embeds/topic-feature-01.png)

## Related articles

- [Understanding [Feature]](UnderstandingFeature)
```

### 3. Wire in & verify

- Add the new page to `mkdocs.yml`'s `nav` section — and **only** that section, following the existing indentation and "Topic Name:" grouping already in place. Don't touch any other part of `mkdocs.yml`.
- Don't edit `docs/_static`, `site/`, `venv/`, `requirements.txt`, or any top-level file other than the `nav` block, per `docs/styleguide.md`.
- Before presenting the draft, self-check it against this list:
  - [ ] Filename and folder match the naming conventions.
  - [ ] Front matter tags are all from the approved list.
  - [ ] H1/H2 casing and blank lines are correct.
  - [ ] Buttons/interface features/fields/code use the right formatting (quotes/bold/italics/code).
  - [ ] "Select" used instead of "click"; no stray `-` separators.
  - [ ] Screenshots (if any) sit below their text with real alt text.
  - [ ] Nav entry added in the right place in `mkdocs.yml`.
  - [ ] A reader unfamiliar with this specific feature, but familiar with Mukurtu generally, could follow the steps without needing the screenshot.
