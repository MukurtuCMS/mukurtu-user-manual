---
tags:
    - roundtrip
    - media
---

# Importing Media Assets

!!! Roles "User roles" 
    Administrator, Mukurtu manager, Roundtrip manager

## Overview

To import media assets, users will use both upload fields on the import page. The **Metadata Files** field is for CSV files and is where users provide their media asset metadata. The **Media/Binary Files** field where useres upload the associated media or binary files.  

!!! Requirement
    To upload media, you must upload an accompanying media asset metadata sheet. 

1. Select "Browse" from the **Metadata Files** field, then select the file(s) you would like to upload. Different media asset types require different CSV files.
2. Select "Browse" from the **Media/Binary Files** field. Select the media file(s) you would like to upload.

Any combination of CSV sheets and supported media assets can be selected. When you are done, select "Next" to continue on to the file configuration page. Media asset metadata imports are configured the same way as content. For specific instructions on how to configure imports, refer to the [Configure Import Settings section of the Importing Content](ImportingContent.md#configure-import-settings) article.

## Media types and core metadata fields

For most media imports, the following fields are the most relevant. Technical metadata fields, which apply to all media types but are not generally required for most imports, are outlined in the [Technical Metadata Fields](#technical-metadata-fields) section of this article.

You can also access this information within your site following the instructions at [General Import Information - Import Templates](GeneralImportInformation.md#import-templates). 

!!! Note
    Semicolon (;) is the default delimiter in all multi-value fields.

### Audio

**Supported file formats:** mp3, m4a, wav, ogg, aac

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Audio file|    |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|Name|Will autofill from the filename. This field is not usually shown to end users. While the media name can be changed, we generally recommend using the auto-filled names so that they match your other records and systems.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the audio file. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. |Plain text, maximum 255 characters.|
|Transcription|A short text transcription of the audio file. This is used as the corresponding text when the audio file is used as a sample sentence in a dictionary word.|Plain text, maximum 255 characters.|
|Contributor|Speakers or singers present in the audio file. Contributors listed here are displayed in the speaker field that accompanies the audio file in dictionary words.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Optional**|**Rarely used**|   |
|Thumbnail > File ID|Audio files are usually represented by an interactive audio player, with a thumbnail image used in certain contexts. When the thumbnail image is used, you can provide your own image instead of the generic thumbnail. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### Document

**Supported file formats:** pdf, txt, rtf, doc, docx, ppt, pptx, xls, xlsx, odf, odg, odp, ods, odt, fodt, fods, fodp, fodg, key, numbers, pages, csv, sxw, zip, rar, gz, 7z, tar

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Document|  |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|Name|Will autofill from the filename. his field is not usually shown to end users. While the media name can be changed, we generally recommend using the auto-filled names so that they match your other records and systems.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the document. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|
|**Optional**|**Rarely used**|   |
|Thumbnail > File ID|A thumbnail image showing the first page of the document is automatically generated and is normally used, with a generic image used in certain contexts. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|
|Extracted text|OCR or other embedded text from the uploaded file. This should be automatically processed.|Formatted text.|

### External embed

**Supported file formats:** No separate file, usually code wrapped in `<iframe></iframe>` tags.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Name|The displayed name of the external embed.|Plain text.|
|External embed|Embed code from an external website. Note that while the media asset will be managed by cultural protocols, the originating website may not have similar privacy settings. External embeds are usually some kind of code wrapped in `<iframe></iframe>` tags.|Formatted text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|Thumbnail > File ID|External embeds usually display the content of the embed, with a thumbnail image used in certain contexts. Thumbnail images must be provided for external embeds, and are often a screenshot of the embedded content.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the embed. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|

### Image

**Supported file formats:** jpeg, jpg, png, gif, webp

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Image > File ID|  |The file ID or filename of the uploaded file.|
|Image > Alternative Text|  |Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|Name|Will autofill from the filename. This field is not usually shown to end users. While the media name can be changed, we generally recommend using the auto-filled names so that they match your other records and systems.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Rarely used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the image. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|

### Remote video

**Supported file formats:** YouTube or Vimeo URLs.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Video URL|A video hosted on Vimeo or YouTube. The remote video will stream using Vimeo or YouTube's media player, and is not copied to the site. Note that while the media asset will be managed by cultural protocols, the originating website may not have similar privacy settings.|Plain text (Vimeo or YouTube URL).|
|Name|Will autofill but manual entry is recommended, especially for larger imports.|Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the video. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|
|**Optional**|**Rarely used**|   |
|Thumbnail > File ID|Videos are usually represented by an interactive video player, with a thumbnail image used in certain contexts. When the thumbnail image is used, you can provide your own image instead of the generic thumbnail. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### SoundCloud

**Supported file formats:** SoundCloud URLs.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|SoundCloud URL|A track, playlist, or album hosted on SoundCloud. The remote file will stream using SoundCloud's media player, and is not copied to the site. Note that while the media asset will be managed by cultural protocols, the originating website may not have similar privacy settings.|Plain text (SoundCloud URL).|
|Name|Will autofill but manual entry is recommended, especially for larger imports.|Plain text.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the recording. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|
|Contributor|Speakers or singers present in the audio file. Contributors listed here are displayed in the speaker field that accompanies the audio file in dictionary words.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Optional**|**Rarely used**|   |
|Thumbnail > File ID|SoundCloud audio is usually represented by an interactive audio player, with a thumbnail image used in certain contexts. When the thumbnail image is used, you can provide your own image instead of the generic thumbnail. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
|Thumbnail > Alternative text|   |Alt text for the thumbnail (required if a thumbnail is included).|

### Video

**Supported file formats:** mp4, webm, ogv.

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**|  |
|Video file|  |The file ID or filename of the uploaded file.|
|Cultural Protocols > Protocols|   |IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting|   |Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing media, not when creating new media.|Integer.|
|**Required**|**Will autofill if empty**|   |
|Name|Will autofill from the filename. This field is not usually shown to end users. While the media name can be changed, we generally recommend using the auto-filled names so that they match your other records and systems.|Plain text.|
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Optional**|**Commonly used**|   |
|Media tags|Media tags are used to label media assets to help find them within the media library. They are also used to trigger taxonomy based media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|People|A person or people present or referenced in the video. This is used to trigger deceased person media content warnings.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier|A unique, unambiguous reference to the media asset. Identifiers are often provided by the contributing institution or organization so the original item can be located. Examples include call numbers or accession numbers. |Plain text, maximum 255 characters.|
|**Optional**|**Rarely used**|   |
|Thumbnail > File ID|Videos are usually represented by an interactive video player, with a thumbnail image used in certain contexts. When the thumbnail image is used, you can provide your own image instead of the generic thumbnail. A thumbnail image does not usually need to be provided.|The file ID or filename of the uploaded image.|
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