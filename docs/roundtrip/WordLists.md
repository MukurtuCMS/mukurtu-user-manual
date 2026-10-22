---
tags: 
    - roundtrip
    - content
    - metadata
---
# Importing Word Lists

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

CSV templates can be downloaded from your own site at `/admin/import/format` (linked on the dashboard as "Import format information"). For more information on word lists metadata fields, refer to [Create a Word List](../dictionary/WordLists.md).

## Word lists

|Field Name|Description|Format Information|
|---|---|---|
|**Mukurtu Essentials Required Fields**|**Cannot be empty**||
|Word list name|A short, descriptive name for the word list. The name should give users useful information about the word list when browsing or searching.|This field is plain text and limited to 255 characters.|
|Cultural protocols > Protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting||Either 'Any' or 'All', case insensitive.|
|**Mukurtu Essentials**|
|Summary|A short summary of the word list. The summary should supplement the title. The summary is displayed as part of the word list preview when browsing the site.|This field is plain text and limited to 255 characters.|
|Description|The explanation or definition of the word list. The description may include guidance on use, explanation of word selection or arrangement, or any other contextual information.|Formatted text.|
|Words|The words included in the word list.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Image|A featured image that is used on the word list page and in previews across the site.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Source|Source provides a reference to the organization or individual responsible for the holding, description, origination, or contribution of the word list. Examples include institutions (e.g.,: "Library of Congress, American Folklife Center"), or donors (e.g.,: "Donated by John Smith").|This field is plain text and limited to 255 characters.|
|**Additional Fields**|
|Keywords|Keywords are used to tag word lists to ensure they are discoverable when searching or browsing. Include as many keywords as needed.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points|A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a word list. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools. Note that this mapping data will be shared with the same users or visitors as the rest of the word list. If the location is sensitive, carefully consider using this field.|The data is stored in a GeoJSON format.|
|Location description|A descriptive field to provide additional context and depth to the location(s) connected to the word list.|Formatted text.|
|Location (taxonomy)|A named place, or places, that are closely connected to the word list. Include as many locations as needed.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts Projects|This field will apply all of the Labels from the selected Local Contexts Project(s) to the collection.|Project titles or IDs, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices|This field allows selective application of one or more Labels from any available Local Contexts Project to the collection.|Label or notice names, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content|Word lists can be related to any other site content when there is a connection that is important to show. Eg: a digital heritage lesson plan that is supplemented by the word list. Note that this field is not used to indicate words in the word list. See the words field instead.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
