---
tags: 
    - roundtrip
    - content
    - metadata
---
# Import Dictionary Words

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

This article provides some general notes and tips to help you get the most out of importing Dictionary Words using Roundtrip. 

## Dictionary Words Notes and Tips

- If including **Sample Sentences** and **Word Entries**, the Dictionary Word CSV and associated paragraph CSVs must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraphs to the proper dictionary word. 
- When importing your CSV files, they should be ordered Dictionary Word CSV, then the individual paragraph CSVs. This ensures the person record is created before the paragraphs. The paragraph CSVs can be in any order.
- You can use the same CSV for sample sentences that are in the main entry and in word entries. To do this, ensure they are connected properly via an ID.

## Technical Metadata Fields

### Dictionary Word CSV

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Term||This field is plain text and limited to 255 characters.|
|Cultural protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Sharing setting||Either 'Any' or 'All', case insensitive.|
|Language||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary.|
|**Mukurtu Essentials**|
|Glossary Entry||This field is plain text and limited to 255 characters.|
|Alternate Spelling||This field is plain text and limited to 255 characters.|
|Translation||This field is plain text and limited to 255 characters, separated by your selected multi-value delimiter.|
|Recording||ID, UUID, or title of the reference. The title must be exact and match only one item.|
|Definition||Formatted text.|
|Sample Sentences||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Word Type||Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Pronunciation||Formatted text.|
|Source||This field is plain text and limited to 255 characters.|
|Word Origin||This field is plain text and limited to 255 characters.|
|Contributor||Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Word Entries**|
|Word Entry||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Thumbnail||ID, UUID, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Media assets||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Keywords||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points||The data is stored in a GeoJSON format.|
|Location description||Formatted text.|
|Location (taxonomy)||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts projects||Local Contexts Project ID values, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices||Local Contexts Project ID:Label/Notice ID values, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

### Paragraphs - Sample Sentences CSV

|Field Name|Format Information|
|---|---|
|Sample Sentence|Plain text value.|
|Recording|ID, UUID, or title of the reference. The title must be exact and match only one item.|

### Paragraphs - Word Entry CSV

|Field Name|Format Information|
|---|---|
|Term|This field is plain text and limited to 255 characters.|
|Alternate Spelling|This field is plain text and limited to 255 characters.|
|Translation|This field is plain text and limited to 255 characters, separated by your selected multi-value delimiter.|
|Recording|ID, UUID, or title of the reference. The title must be exact and match only one item.|
|Definition|Formatted text.|
|Sample Sentences|The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Word Type|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Pronunciation|Formatted text.|
|Source|This field is plain text and limited to 255 characters.|
|Word Origin|This field is plain text and limited to 255 characters.|
|Contributor|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
