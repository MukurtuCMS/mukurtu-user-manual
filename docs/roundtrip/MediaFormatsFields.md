---
tags:
    - roundtrip
    - media
---

# Media Formats and Fields

!!! Roles "User roles" 
    TBD

## Media types and core metadata fields

For most media imports, the following fields are the most relevant. More technical fields, which apply to all media types but are not generally required for most imports, are presented separately.

You can also access this information within your site following the instructions at [Import Format Information](ImportFormatInformation.md). 

!!! Note
    Semicolon (;) is the default delimiter in all multi-value fields.

### Audio

**Supported file formats:** mp3, m4a, wav, ogg, aac.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**| | |
|Audio file|    |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill from the filename. This field is not usually shown to end users. While the media name can be changed, we generally recommend using the auto-filled names so that they match your other records and systems.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the audio file. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. |Plain text, maximum 255 characters.|
|Transcription|A short text transcription of the audio file. This is used as the corresponding text when the audio file is used as a sample sentence in a dictionary word.|Plain text, maximum 255 characters.|
|Contributor|Contributor	Speakers or singers present in the audio file. Contributors listed here are displayed in the speaker field that accompanies the audio file in dictionary words.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|Audio files are usually represented by an interactive audio player, with a thumbnail image used in certain contexts. When the thumbnail image is used, you can provide your own image instead of the generic thumbnail. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### Document

**Supported file formats:** pdf, txt, rtf, doc, docx, ppt, pptx, xls, xlsx, odf, odg, odp, ods, odt, fodt, fods, fodp, fodg, key, numbers, pages, csv, sxw, zip, rar, gz, 7z, tar.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**| | |
|Document|  |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill with the filename given in the *document* field.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|
|Extracted text|    |   |

### External embed

**Supported file formats:** No separate file, usually code wrapped in `<iframe></iframe>` tags.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**| | |
|Name|  |Plain text.|
|External embed|    |   |
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|

### Image

**Supported file formats:** jpeg, jpg, png, gif, webp.

|Field Name|Description|Format Information|
|---|---|---|
|Image > File ID|  |The file ID or filename of the uploaded file.|
|Image > Alternative Text|  |Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill with the filename given in the *document* field.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|

### Remote video

**Supported file formats:** YouTube or Vimeo URLs.

|Field Name|Description|Format Information|
|---|---|---|
|Video URL|  |  |
|Name|Will autofill but manual entry is recommended, especially for larger imports.|Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### SoundCloud

**Supported file formats:** SoundCloud URLs.

|Field Name|Description|Format Information|
|---|---|---|
|SoundCloud URL|  | |
|Name|Will autofill but manual entry is recommended, especially for larger imports.|Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill with the filename given in the *document* field.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|
|Contributor|   |   |
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### Video

**Supported file formats:** mp4, webm, ogv.

|Field Name|Description|Format Information|
|---|---|---|
|Video file|  |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required, but will autofill if empty**|   |   |
|Name|Will autofill with the filename given in the *document* field.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional (commonly used)**|   |   |
|Media tags|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|   |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|   |Plain text.|
|**Optional (rarely used)**|   |   |
|Thumbnail > File ID|   |The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

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





