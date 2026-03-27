---
tags: 
    - roundtrip
    - content
    - metadata
---
# Import Collections

!!! roles "User roles"
    Administrator, Mukurtu manager, Mukurtu roundtrip manager

This article provides some general notes and tips to help you get the most out of importing Collections using Roundtrip. 

## Collections Notes and Tips

- When importing complex collections that have subcollections, the subcollections must be created first. Therefore, subcollections should be ordered first in the spreadsheet above any parent collections. 
- Collections do not have paragraphs.
- Content must exist to be added to Collections.

## Technical Metadata Fields

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Collection name||This field is plain text and limited to 255 characters.|
|Cultural protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Sharing setting||Either 'Any' or 'All', case insensitive.|
|**Mukurtu Essentials**|
|Summary||This field is plain text and limited to 255 characters.|
|Description||Formatted text.|
|Image||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Source||This field is plain text and limited to 255 characters.|
|Items in Collection||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Sub-Collections||IDs or UUIDs of the references, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points||The data is stored in a GeoJSON format.|
|Location description||Formatted text.|
|Location (taxonomy)||Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts projects||Local Contexts Project ID values, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices||Local Contexts Project ID:Label/Notice ID values, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content||IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
