---
tags: 
    - roundtrip
    - content
    - metadata
---
# Importing Place Records

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Import templates can be created and downloaded from your own site at `/admin/import/format` (linked on the dashboard as "Import format information"). For more information on place records metadata fields, refer to [Create Place Records](../place-records/CreatePlaceRecord.md).

## Place records

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**||
|Name|The place, as it should be primarily identified.|This field is plain text and limited to 255 characters.|
|Cultural protocols > Protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting||Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing person records, not when creating new person records.|Integer.|
|**Required**|**Will autofill if empty**||
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Mukurtu Essentials**|
|Other Place Names|Places may be identified by multiple names, monikers, identities, and with inconsistent spellings across different content. This field is used to aggregate and display all content where the place is identified by connecting those disparate names. Include as many place names as needed. |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Media assets|Media assets are a key element of most place records, though they are not required. Supported media types are images, documents, video, audio, and embed code. Place records can include more than one media asset, and each media asset can be a different media type. Media assets can be assigned a different cultural protocol from the place record to allow differential access to the media assets and metadata. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Place type|Place types are used to tag place records to indicate different types of locations or places. Include as many place types as needed.|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points|A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a place record. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools. Note that this mapping data will be shared with the same users or visitors as the rest of the place record. If the location is sensitive, carefully consider using this field.|The data is stored in a GeoJSON format.|
|Location description|A descriptive field to provide additional context and depth to the location(s) connected to the place record. |Formatted text.|
|Location (taxonomy)|A named place, or places, that are closely connected to the place record. Include as many locations as needed. |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Text Sections**|
|Text section|A description of the history, significance, or other information about the place highlighted in the place record.|The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords| 	Keywords are used to tag place records to ensure that they are discoverable when searching or browsing. Include as many keywords as needed. |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts Projects|This field will apply all of the Labels from the selected Local Contexts Project(s) to the place record. |Project titles or IDs, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices|This field allows selective application of one or more Labels from any available Local Contexts Project to the place record.|Label or notice names, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content|Place records can be related to any other site content when there is a connection between those items that is important to show. Note that the place record will automatically aggregate all content where the place is referenced based on the representative terms field, and manually managing related content may not be necessary. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

## Text Sections

Text sections is a group of repeatable fields that are handled as "paragraphs" in import. To include this citation, you will need to include corresponding spreadsheets as well. That spreadsheet is included in this article, but please review [General Import Information > Importing Paragraphs](../roundtrip/GeneralImportInformation.md/#paragraphs) for more information on how to format and connect the spreadsheets during an import.

If including **Text Sections** paragraphs, the Place record CSV and associated paragraph CSV must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraphs to the proper person record. 

|Field Name|Description|Format Information|
|---|---|---|
|Title|The title of the section.|Plain text value.|
|Body|The body of the section.|Formatted text.|
