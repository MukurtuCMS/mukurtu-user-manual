---
tags: 
    - roundtrip
    - content
    - metadata
---
# Import Place Records

!!! roles "User roles"
    Administrator, Mukurtu manager, Mukurtu roundtrip manager

## Technical Metadata Fields

### Place record CSV

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Name||This field is plain text and limited to 255 characters.|
|Cultural protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Sharing setting||Either 'Any' or 'All', case insensitive.|
|**Mukurtu Essentials**|
|Other Names||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Media assets||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Map points||The data is stored in a GeoJSON format.|
|Location description||Formatted text.|
|Location (taxonomy)||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Text Sections**|
|Text section||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts projects||Local Contexts Project ID values, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices||Local Contexts Project ID:Label/Notice ID values, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

### Paragraphs - Text section CSV

|Field Name|Format Information|
|---|---|
|Title|Plain text value.|
|Body|Formatted text.|