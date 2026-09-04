---
tags: 
    - roundtrip
    - content
    - metadata
---
# Importing Person Records

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

CSV templates can be downloaded from your own site at `/admin/import/format` (linked on the dashboard as "Import format information"). For more information on person records metadata fields, refer to [Create Person Records](../person-records/PersonRecords.md).

## Person records

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**||
|Name|The person's name, as they should be primarily identified.|This field is plain text and limited to 255 characters.|
|Cultural protocols > Protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting||Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing person records, not when creating new person records.|Integer.|
|**Required**|**Will autofill if empty**||
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Mukurtu Essentials**|
|Other Names|People may be identified by multiple names, monikers, identities, and with inconsistent spellings across different content. This field is used to aggregate and display all content where the person is identified by connecting those disparate names. Include as many names as needed.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Media assets|Media assets are a key element of most person records, though they are not required. Supported media types are images, documents, video, audio, and embed code. Person records can include more than one media asset, and each media asset can be a different media type. Media assets can be assigned a different cultural protocol from the person record to allow differential access to the media assets and metadata.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Date born|The date the person was born.|YYYY, YYYY-MM, or YYYY-MM-DD value.|
|Date died|The date the person died.|YYYY, YYYY-MM, or YYYY-MM-DD value.|
|Deceased|Indicates if the person is deceased or not. If the deceased person media content warning is configured, warnings will be displayed based on this field.|Boolean (0 or 1) value.|
|Place of birth|The place where the person was born.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Place of death|The place where the person died.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Biography**|
|Related People||The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Biography|The biography is an account of the person's life, whether written or compiled by others, an autobiography, or both. While they are primarily written, they may include media assets as well. Biographies can be composed in sections to more clearly structure the person's life events, story, accomplishments, and relationships. |The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords| 	Keywords are used to tag person records to ensure that they are discoverable when searching or browsing. Examples include significant life events or organizations which the person was involved with. Include as many keywords as needed.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points|A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a person record. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools. Note that this mapping data will be shared with the same users or visitors as the rest of the person record. If the location is sensitive, carefully consider using this field.|The data is stored in a GeoJSON format.|
|Location description|A descriptive field to provide additional context and depth to the location(s) connected to the person record.|Formatted text.|
|Location (taxonomy)|A named place, or places, that are closely connected to the person record. Examples include the places a person was born, lived, died, or sites of important life events.
Include as many locations as needed.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts Projects|This field will apply all of the Labels from the selected Local Contexts Project(s) to the person record.|Project titles or IDs, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices|This field allows selective application of one or more Labels from any available Local Contexts Project to the person record.|Label or notice names, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content|Person records can be related to any other site content when there is a connection between those items that is important to show. Note that the person record will automatically aggregate all content where the person is referenced based on the representative terms field, and manually managing related content may not be necessary.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

## Related People and Biography Sections

Related People and Biography sections are a group of repeatable fields that are handled as "paragraphs" in import. To include this citation, you will need to include corresponding spreadsheets as well. Those spreadsheets are included in this article, but please review [General Field Information > Importing Paragraphs](../roundtrip/GeneralImportInformation.md/#paragraphs) for more information on how to format and connect the spreadsheets during an import.

If including **Related People** and **Biography Section** paragraphs, the Person record CSV and associated paragraph CSV must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraphs to the proper person record. 

### Related People

|Field Name|Description|Format Information|
|---|---|---|
|Import ID, ID, or UUID|When importing a person record and corresponding related people paragraph at the same time, use an *Import ID*|See [General Field Information > Identifiers](./GeneralImportInformation.md#identifiers-name-id-uuid-import-id) for more information.|
|Related Person|A person that has a relationship with the subject of the person record. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Relationship type|The type of relationship between the related person and the subject of the person record.|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|

### Biography Section

|Field Name|Description|Format Information|
|---|---|---|
|Import ID, ID, or UUID|When importing a person record and corresponding biography section paragraph at the same time, use an *Import ID*|See [General Field Information > Identifiers](./GeneralImportInformation.md#identifiers-name-id-uuid-import-id) for more information.|
|Title|The title of the section.|Plain text value.|
|Body|The body of the section.|Formatted text.|
