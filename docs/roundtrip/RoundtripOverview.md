---
tags:
    - roundtrip
---

# Roundtrip Overview

!!! Roles "User roles" 
    Administrator, Mukurtu manager, Roundtrip manager

Roundtrip is the collection of tools we use for import and export of site content (content, media, taxonomies, basically anything). It serves several purposes:

- Bulk ingesting new content.
- Bulk updating content.
- Exporting content to share with another site/organization.
- Exporting content for a backup/reference.

![Slide1](../_embeds/RoundtripSlide1.jpg)

![Slide2](../_embeds/RoundtripSlide2.jpg)

From Mukurtu 2 onwards we have focused on UTF-8 encoded CSV sheets for import/export. This is to ensure that we avoid proprietary formats and work with the most basic and transportable data format available. Yes, this has created some complications with Excel users in the past... https://mukurtu.org/support/file-formats-character-encoding-and-spreadsheet-tools/

Bulk ingest/export of media assets and metadata for basically all site content/entities/components must be supported.
