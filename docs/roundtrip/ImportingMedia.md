---
tags:
    - roundtrip
    - media
---

# Importing Media

!!! Roles "User roles" 
    TBD

## Supported file formats

The following list is the media file formats supported by the stock Mukurtu installation.

**Audio:** mp3, m4a, wav, ogg, aac.

**Document:** pdf, txt, rtf, doc, docx, ppt, pptx, xls, xlsx, odf, odg, odp, ods, odt, fodt, fods, fodp, fodg, key, numbers, pages, csv, sxw, zip, rar, gz, 7z, tar.

**External embed:** No separate file, usually code wrapped in `<iframe>` tags.

**Image:** jpeg, jpg, png, gif, webp.

**Remote video:** YouTube or Vimeo URLs.

**SoundCloud:** SoundCloud URLs.

**Video:** mp4, webm, ogv.

## Basic metadata fields

For most media imports, the following fields are the most relevant. More technical fields, which apply to all media types but are not generally required for most imports, are presented separately.

You can also access this information within your site following the instructions at [Import Format Information](ImportFormatInformation.md). 

**Audio**

- Required
    - Audio file
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - Name (from Audio file)
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier
    - Transcription
    - Contributor
- Optional (uncommon)
    - Thumbnail > File ID (uses a player or a generic thumbnail)
    - Thumbnail > Alternative Text

**Document** 

- Required
    - Document
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - Name (from Document)
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier
- Optional (uncommon)
    - Thumbnail > File ID (should be automatic)
    - Thumbnail > Alternative Text (should be automatic)
    - Extracted text (should be automatic)

**External embed**

- Required
    - Name
    - External Embed
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - Thumbnail > File ID
    - Thumbnail > Alternative Text
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier

**Image**

- Required
    - Image > File ID
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - Name (from Image > File ID)
    - Image > Alternative Text (from Image > File ID)
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier

**Remote video**

- Required
    - Video URL (YouTube, Vimeo)
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - Name (should autofill, but manual entry is recommended, especially for larger imports)
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier
- Optional (uncommon)
    - Thumbnail > File ID (should be automatic, defaults to a player)
    - Thumbnail > Alternative Text (should be automatic)

**SoundCloud**

- Required
    - SoundCloud URL
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - Name (should autofill, but manual entry is recommended)
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - UUID (if creating new media)
- Optional (common)
    - Media Tags
    - People
    - Identifier
    - Contributor
- Optional (uncommon)
    - Thumbnail > File ID (should be automatic, defaults to a player)
    - Thumbnail > Alternative Text (should be automatic)

**Video**

- Required
    - Video file
    - Cultural Protocols > Protocols
    - Cultural Protocols > Sharing Setting
    - ID (ONLY if updating existing media)
- Required, but will autofill if empty
    - UUID (if creating new media)
    - Name (from Video file)
- Optional (common)
    - Media Tags
    - People
    - Identifier
- Optional (uncommon)
    - Thumbnail > File ID (uses a player or a generic thumbnail)
    - Thumbnail > Alternative Text

## Technical Metadata Fields

- Language (langcode)
- Revision create time
- Revision user
- Revision log message
- Published
- Authored by
- Authored on
- Changed
- Default translation
- Default revision

## Import Process