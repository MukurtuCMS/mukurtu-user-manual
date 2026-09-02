---
tags:
    - roundtrip
---

# Exporting Media

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Media assets, images, audio, video, and other files attached to your content, can be exported on their own, in addition to being included automatically when you export the content they belong to. This article covers both. For the general export process, see [Exporting Content](ExportingContent.md); for what the settings below control, see [Export Settings](ExportSettings.md).

!!! requirement
    Users must be an Administrator, Mukurtu manager, or Roundtrip manager to access export tools.

## Add media to an export list

Media items don't have their own full page with an "Add to Export List" option the way content does. Instead, add media to an export list from the media library.

From your **Dashboard**, under **Media**, select **Manage Media**.

- To add a single item, select "Add to export list" from its actions menu, or, if it's shown directly on the item, select the "Add to export list" toggle.
- To add multiple items at once, select the items you want, then choose "Add to Export List" from the bulk actions menu.

Both work the same way as adding content: you'll choose an existing export list, or create a new one. See [Add a single item](ExportingContent.md#add-a-single-item) for that form.

!!! tip
    Select "Export" from a media item's actions menu to export just that item right away, without adding it to a list first.

## Media included with content

When you export content whose *Media* setting (see [Configuration](ExportSettings.md#configuration)) is set to include the referenced media, that media is exported automatically along with it. It isn't folded into the content's own row: each media type exports to its own file (for example, `Media - Image.csv`), using that type's own field mapping. You don't need to separately add that media to your export list for this to happen.

## Media asset packaging

Whether the actual file is bundled with the export, or just an identifier, is controlled by *Media asset packaging* in the export setting you use (see [Configuration](ExportSettings.md#configuration)). This only matters for media types that store a local file: Image, Audio, Video, and Document. Remote Video, SoundCloud, and External Embed store a URL or embed code instead of a file, so this setting has no effect on them.

## Supported media types

Mukurtu can export all of its media types: Image, Audio, Video, Document, Remote Video, SoundCloud, and External Embed. Each has its own field mapping table in [Export Settings](ExportSettings.md#field-mappings).
