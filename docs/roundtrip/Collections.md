---
tags: 
    - roundtrip
    - content
    - metadata
---
# Importing Collections

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Import templates can be created and downloaded from your own site at `/admin/import/format` (linked on the dashboard as "Import format information"). For more information on collections metadata fields, refer to [Create Collections](../collections/CreateCollection.md).

- When importing complex collections that have subcollections, the subcollections must be created first. Therefore, subcollections should be ordered first in the spreadsheet above any parent collections. 
- Content must exist to be added to Collections.

## Collections

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**||
|Collection name|A short, descriptive name for the collection. The name should give users useful information about the collection when browsing or searching. |This field is plain text and limited to 255 characters.|
|Cultural protocols > Protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting||Either 'Any' or 'All', case insensitive.|
|ID|Only used when updating existing collections, not when creating new collections.|Integer.|
|**Required**|**Will autofill if empty**||
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Mukurtu Essentials**|
|Summary|A short summary of the collection. The summary should supplement the title. The summary is displayed as part of the collection preview when browsing the site. |This field is plain text and limited to 255 characters.|
|Description|The history, story, explanation, provenance, arrangement information, or other description information about the collection. This is often based on existing collection descriptions and may include finding aids and other supplementary documentation. |Formatted text.|
|Image|A featured image that is used on the collection page and in previews across the site. The image may be drawn from content in the collection, or selected to complement the collection. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Source|Source provides a reference to the organization or individual responsible for the holding, description, origination, or contribution of the collection. Examples include institutions (e.g.,: "Library of Congress, American Folklife Center"), or donors (e.g.,: "Donated by John Smith"). |This field is plain text and limited to 255 characters.|
|Items in Collection|The content found in the collection. Collections most commonly focus on digital heritage items, but content of any type can be included. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Sub-Collections|Large collections may benefit from more internal structure or organization. This is done using sub-collections and may reflect existing physical arrangement (eg: boxes, folders, subfolders), topical groupings, or any other arrangement that will help users navigate the collection. Sub-collections can be multiple levels deep. |IDs or UUIDs of the references, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Keywords|Keywords are used to tag collections to ensure they are discoverable when searching or browsing. |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points|A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a collection. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools. Note that this mapping data will be shared with the same users or visitors as the rest of the collection. If the location is sensitive, carefully consider using this field. |The data is stored in a GeoJSON format.|
|Location description|A descriptive field to provide additional context and depth to the location(s) connected to the collection. |Formatted text.|
|Location (taxonomy)|A named place, or places, that are closely connected to the collection. Examples include the location where a photo was taken, places named in a story, or the site where an object was created. |Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts Projects|This field will apply all of the Labels from the selected Local Contexts Project(s) to the collection. |Project titles or IDs, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices|This field allows selective application of one or more Labels from any available Local Contexts Project to the collection. |Label or notice names, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content|Collections can be related to any other site content when there is a connection that is important to show. Eg: another collection from the same donor. Note that this field is not used to indicate content in the collection. See the items in collection field instead. |IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
