---
tags:
    - roundtrip
    - taxonomies
---

# Importing Taxonomy Terms

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Taxonomy terms, the vocabularies used for categories, languages, media tags, and other structured lists, are imported the same way as content: through the regular import wizard. See [Importing Content](ImportingContent.md) for the general steps.

## Choose a taxonomy import type

When configuring your import, select **Taxonomy** as the import type. Under *import sub-type*, choose the vocabulary you're importing.

!!! tip
    Every vocabulary uses the same fields except Category, so the sub-type list shows only two entries: **Category** and **Other Taxonomies**. Select **Other Taxonomies** regardless of which non-Category vocabulary (Language, Media Tag, Subject, and so on) you're actually importing into — you'll choose the specific vocabulary elsewhere in your import configuration, not from this list.

## Fields

Every vocabulary shares the same core fields:

- *Term ID*: the term's numeric identifier, assigned by the system.
- *Locale*: the term's language code.
- *Name*: the term's label.
- *Description*: optional text, not normally shown to visitors.
- *Parent*: not currently supported in Mukurtu. Omit this field even if your spreadsheet has a column for it.
- *Default translation*: whether this row is the term's default translation.

Category terms also have a *Thumbnail Image* field (File ID and Alternative text).

See [Import Format Information](ImportFormatInformation.md) for the full, current field list for any specific vocabulary.
