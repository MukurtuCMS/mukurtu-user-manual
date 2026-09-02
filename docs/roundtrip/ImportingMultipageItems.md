---
tags:
    - roundtrip
---

# Importing Multipage Items

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Multipage items, such as yearbooks, scrapbooks, or photo albums, can be created and updated in bulk the same way as content, through the regular import wizard. See [Importing Content](ImportingContent.md) for the general steps.

!!! requirement
    Import the pages themselves first, as their own content type, before importing the multipage item that references them.

## Choose the import type

When configuring your import, select **Multipage Item** as the import type.

## Fields

- *Title*: if left blank, this defaults to the title of the first page.
- *Pages*: the content that makes up the item, referenced by their identifiers and separated with your configured multi-value delimiter. Pages appear in the order you list them here.
- *Author*, *Authored on*, *Language*, *Default translation*, *Status*, *ID*, *UUID*: standard metadata and identifier fields, the same as content.

See [Import Format Information](ImportFormatInformation.md) for the full, current field list.
