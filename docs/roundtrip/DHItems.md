---
tags: 
    - roundtrip
    - content
    - metadata
---
# Import Digital Heritage Items

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

This article provides some general notes and tips to help you get the most out of importing Digital Heritage Items using Roundtrip. 

## Digital Heritage Items Notes and Tips

- If including **Citing Indigenous Elders and Knowledge Keepers**, the Digital Heritage Item CSV and paragraph CSV must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraph to the proper digital heritage item. 
- When importing your CSV files, they should be ordered Digital Heritage Item CSV, then the paragraph CSV. This ensures the digital heritage item is created before the paragraph. 

## Technical Metadata Fields

### Digital heritage item CSV

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Title||This field is plain text and limited to 255 characters.|
|Cultural protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Sharing setting||Either 'Any' or 'All', case insensitive.|
|Category||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary.|
|**Mukurtu Essentials**|
|Media assets||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Summary||This field is plain text and limited to 255 characters.|
|Creator||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Contributor||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Original date||YYYY, YYYY-MM, or YYYY-MM-DD value.|
|Date description||This field is plain text and limited to 255 characters.|
|**Mukurtu Core**|
|Cultural narratives||Formatted text.|
|Traditional knowledge||Formatted text.|
|Description||Formatted text.|
|**Permissions and Rights**|
|Local Contexts projects||Local Contexts Project ID values, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices||Local Contexts Project ID:Label/Notice ID values, separated by your selected multi-value delimiter.|
|Citing Indigenous Elders and Knowledge Keepers||The ID or UUID of the paragraph.|
|Rights and Usage||This field is plain text and limited to 255 characters.|
|Rights Statements||The value or the label of allowed values.|
|Creative Commons Licenses||The value or the label of allowed values.|
|**Additional Fields**|
|Type||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Format||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Identifier||This field is plain text and limited to 255 characters.|
|Keywords||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Language||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points||The data is stored in a GeoJSON format.|
|Location description||Formatted text.|
|Location (taxonomy)||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Source||This field is plain text and limited to 255 characters.|
|Publisher||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|External links||The link in Markdown format: `[Title](https://url.com)`, separated by your selected multi-value delimiter. The URL must be formatted as a full URL, such as `https://example.com`, and the link text is a plain text field.|
|Subject||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Transcription||This HTML field can support rich text and embedded media assets using the editing toolbar.|
|People||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Related Content**|
|Related content||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

### Paragraphs - Citing Indigenous Elders and Knowledge Keepers CSV

|Field Name|Format Information|
|---|---|
|Name of the Elder or Knowledge Keeper|This field is plain text and limited to 255 characters.|
|Nation or Community|This field is plain text and limited to 255 characters.|
|Treaty Territory|This field is plain text and limited to 255 characters.|
|City or Community they live in|This field is plain text and limited to 255 characters.|
|A Brief Description or Title of the Teaching|This field is plain text and limited to 255 characters.|
|Date|YYYY, YYYY-MM, or YYYY-MM-DD value.|

