---
tags:
    - roundtrip
---

# Export Settings

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

A CSV export setting is a saved, reusable configuration that controls exactly which fields are included in an export and how the resulting CSV file is formatted. You can save several settings for different purposes, for example one for updating your own site and another for sharing a limited set of fields with an outside institution.

## Default export settings

Mukurtu ships with four ready-to-use CSV export settings, shared with **All export users** so anyone with export access can use them right away. Each combines one of the two *identifier format* choices with one of the two *media asset packaging* choices described under [Configuration](#configuration) below:

| Setting | Identifiers | Media assets | Use it for |
|---|---|---|---|
| Default local settings (metadata only) | ID | Not included | Re-importing to the same site, metadata only |
| Default local settings (with media assets) | ID | Packaged | Re-importing to the same site, including media |
| Default external settings (metadata only) | UUID | Not included | Sharing metadata with an outside institution, no media |
| Default external settings (with media assets) | UUID | Packaged | Sharing with another site or organization, including media |

All four cover every content type, media type, taxonomy term, and other supported entity, so they're a good starting point to duplicate rather than build a setting from scratch.

## Create a CSV export setting

The four default settings export every field for every content type, using a fixed set of choices for how references are exported. Create a custom setting instead when you need something different, for example:

- Exporting only a curated subset of fields, rather than everything.
- Renaming CSV headers to match a specific partner's or tool's expected format.
- Changing how deeply a particular reference type is followed, such as exporting media as just an identifier instead of packaging the full asset.
- Using different CSV formatting, such as a different delimiter, for a specific downstream tool.
- Keeping the setting visible to only you, rather than sharing it with all export users.

From your **Dashboard**, under **Roundtrip**, select **Export Settings**, then select "New CSV export setting".

!!! tip
    You can also duplicate an existing setting as a starting point. Select "Duplicate" next to the setting you want to copy.

### General settings

- *Label*: the name shown when choosing between saved settings.
- *Description*: optional text shown alongside the name.
- **Visibility**: share the setting with "All export users", or keep it visible to "Only me".

![The general settings for a new CSV export setting: Label, Description, and Visibility.](../_embeds/export-settings-general-01.png)

### Field mappings

Fields are grouped by content and media type (Digital Heritage, Dictionary Word, Person, Place, Collection, Word List, Media, Users, Taxonomy Terms, and others). Open a group to see its fields, each with:

- An **Export** checkbox to include or exclude that field.
- Its *CSV header label*, which you can edit to rename the column in the exported file.
- A drag-and-drop *Weight* to reorder columns.

Only fields with **Export** checked are included in the CSV for that content or media type.

![The expanded Digital Heritage field mapping group, listing its fields with Export checkboxes and editable CSV header labels.](../_embeds/export-settings-field-mappings-01.png)

### Configuration

These settings control how references to other content are written in exported cells (for example, a taxonomy term or related content field). They don't affect the exported item's own ID or UUID columns, which are controlled per content type in *Field mappings* above.

- *Select the identifier format to export*: export the **ID** (suitable for importing back into the same site) or the **UUID** (preferable when sharing data with other sites).
- *Referenced content*, *Media*, *Taxonomy Terms*, *Users*, *Paragraphs*, and *Multipage Items* each let you choose how deeply to follow that kind of reference: export just the identifier, or also include the referenced item itself. Content, media, and paragraph references can also be followed recursively (including their own references in turn), and taxonomy terms can be exported by label instead of identifier.

!!! warning
    Following references recursively can produce very large exports. Use it with caution.

- *Media asset packaging* controls whether binary files (audio, video, documents, images, and thumbnails) are bundled with the export when media is included, and whether the file's own metadata is exported as well.

![The Configuration section, showing the identifier format and reference-depth options.](../_embeds/export-settings-configuration-01.png)

### CSV file format settings

- *Field delimiter*: separates columns. Defaults to a comma (`,`).
- *Field enclosure*: wraps field values. Defaults to a double quote (`"`).
- *Escape character*: escapes the enclosure character within a value. Defaults to a backslash (`\`).
- *Multi-value delimiter*: separates multiple values within a single field. Defaults to a semicolon (`;`).
- *Local Contexts delimiter*: separates parts of an exported Local Contexts label or notice value. Defaults to `>`.
- *Default text format*: the text format exported content is written in. Set the matching import template to the same value.

![The CSV File Format Settings section, showing the field delimiter, enclosure, escape character, and other formatting fields.](../_embeds/export-settings-csv-format-01.png)

Select "Save" when done.

## Manage saved CSV export settings

Users with the *Administer Import Templates* permission can select "Manage saved CSV export settings" from the export page to see every saved setting, its visibility, and description in one place, with actions to edit, duplicate, or delete each one.

![The CSV Exporter Settings page listing a saved setting named Standard export.](../_embeds/export-settings-collection-01.png)

## Related articles

- [Exporting Content](ExportingContent.md)
- [Exporting Media](ExportingMedia.md)
- [Roundtrip Overview](RoundtripOverview.md)
