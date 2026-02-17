---
tags:
    - roundtrip
    - media
---

# Media Formats and Fields

!!! Roles "User roles" 
    TBD

## Supported file formats

The following list is the media file formats supported by the stock Mukurtu installation.

**Audio:** mp3, m4a, wav, ogg, aac.

**Document:** pdf, txt, rtf, doc, docx, ppt, pptx, xls, xlsx, odf, odg, odp, ods, odt, fodt, fods, fodp, fodg, key, numbers, pages, csv, sxw, zip, rar, gz, 7z, tar.

**External embed:** No separate file, usually code wrapped in `<iframe></iframe>` tags.

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
        - If creating new media, the filename included in the import.
        - If updating existing media, the ???
    - Cultural Protocols > Protocols
        - 	IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.
    - Cultural Protocols > Sharing Setting
        - 	Either 'Any' or 'All', case insensitive.
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

|Field Name|Description|Format Information|
|---|---|---|
|**Required**| | |
|Audio file|Allowed file formats are mp3, m4a, wav, ogg, and aac.|The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|   |Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill with the filename given in the *audio file* field.|Plain text.|
|UUID|   |UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|
|Transcription|A short text transcription of the audio file. This is used as the corresponding text when the audio file is used as a sample sentence in a dictionary word.|Plain text, maximum 255 characters.|
|Contributor|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

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

|Field Name|Description|Format Information|
|---|---|---|
|Language (langcode)|   |Language code value.|
|Revision create time|The time that the current revision was created.|Unix timestamp value.|
|Revision user|The user ID of the author of the current revision.|The username or user ID.|
|Revision log message|Briefly describe the changes you have made.|Plain text.|
|Published| |Boolean (0 or 1) value.|
|Authored by|The user ID of the author.|The username or user ID.|
|Authored on|The time the media item was created.|Unix timestamp value.|
|Changed|The time the media item was last edited.|Unix timestamp value.|
|Default translation|A flag indicating whether this is the default translation.|Boolean (0 or 1) value.|
|Default revision|A flag indicating whether this was a default revision when it was saved.|Boolean (0 or 1) value.|





