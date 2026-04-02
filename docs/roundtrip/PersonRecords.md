---
tags: 
    - roundtrip
    - content
    - metadata
---
# Import Person Records

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

This article provides some general notes and tips to help you get the most out of importing Person Records using Roundtrip. 

## Person Records Notes and Tips

- If including **Related People** and **Biography Sections**, the Person record CSV and associated paragraph CSVs must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraphs to the proper person record. 
- When importing your CSV files, they should be ordered Person Record CSV, then the individual paragraph CSVs. This ensures the person record is created before the paragraphs. The paragraph CSVs can be in any order.

## Technical Metadata Fields

### Person record CSV

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Name||This field is plain text and limited to 255 characters.|
|Cultural protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Sharing setting||Either 'Any' or 'All', case insensitive.|
|**Mukurtu Essentials**|
|Other Names||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Media assets||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Date born||YYYY, YYYY-MM, or YYYY-MM-DD value.|
|Date died||YYYY, YYYY-MM, or YYYY-MM-DD value.|
|Deceased||Boolean (0 or 1) value.|
|Place of birth||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Place of death||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Biography**|
|Related People||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Biography||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points||The data is stored in a GeoJSON format.|
|Location description||Formatted text.|
|Location (taxonomy)||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts projects||Local Contexts Project ID values, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices||Local Contexts Project ID:Label/Notice ID values, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

### Paragraphs - Related People CSV

|Field Name|Format Information|
|---|---|
|Related Person|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Relationship type|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|

### Paragraphs - Biography section CSV

|Field Name|Format Information|
|---|---|
|Title|Plain text value.|
|Body|Formatted text.|
