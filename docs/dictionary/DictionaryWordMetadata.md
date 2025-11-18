---
tags:
    - dictionary
---
# Dictionary Word Metadata

!!! roles "User roles"
    Protocol steward, language steward, language contributor

This article provides detail for each of the dictionary word metadata fields. All the information here is presented in the helper text within the dictionary word edit/creation screen. 

## Mukurtu Essentials

### Term
A word, term, phrase, or other language element.

This field is plain text and limited to 255 characters.

### Cultural Protocols
Cultural protocols determine which users can access this content. Cultural protocols are managed by their parent community, which represents a group of contributors. All content must be assigned at least one cultural protocol. Most content only requires one cultural protocol, but more granular access can be specified by selecting multiple protocols, or even protocols from multiple communities.

IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.

### Sharing Setting
Sharing setting determines which users can access this content when multiple cultural protocols are selected. The more restrictive "all cultural protocols" is the default setting, and can be used when only one cultural protocol is selected.

All: This item may only be shared with users who are members of  ALL selected cultural protocols (more restrictive).
Any: This item may be shared with users who are members of ANY one or more selected cultural protocol (less restrictive).

Either 'Any' or 'All', case insensitive.

### Language
Each dictionary word is associated with one language. Dictionary languages must first be configured by a Mukurtu Manager.

IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.

### Glossary Entry
By default, the dictionary word will be indexed, sorted, or alphabetized by the first character of the term. The glossary entry is used for indexing when a character or letter other than the first character in the term should be referenced. Examples include diacritic or accent-initial words, root word markers at the start of the term, or combined characters (eg: ch or á in some languages are considered a single character).

Plain text. 255 characters.

### Alternate Spelling
An alternate spelling of the term. Examples include historic or current variant spellings, spellings from different dialects or in different writing systems, or any other alternate spelling that will help find the dictionary word when searching.

Plain text. 255 characters.

### Translation
Translations of the entry into other languages. Consider indicating the language of the translation, eg: Apple (English).

Plain text. 255 characters. Separated by your selected multi-value delimiter.

### Recording
Audio recordings of the entry being spoken, usually on its own. Multiple recordings may be used to represent different types of speakers (eg: speakers of different ages, genders, accents, or dialects), or different forms the entry can take. 
Recordings can be assigned a different cultural protocol from the dictionary word to allow differential access to the recordings and metadata.

IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.

### Definition
A longer definition or description of the entry. 

Formatted text.

### Sample Sentence
Text entry of the sample sentence.

Plain text. 255 characters.

#### Recording
Audio recording of the sample sentence. Recordings can be assigned a different cultural protocol from the dictionary word to allow differential access to the recordings and metadata.

IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.

### Word Type
Word types may include parts of speech, syntactic or grammatical categories, or any other relevant system to classify entries.

Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.

### Pronunciation
A pronunciation guide used to teach language learners the correct pronunciation of the entry. Pronunciation guides may use a standard phonetic alphabet or whatever notation system is used by speakers and teachers of the language, eg: indicating stress with bold text or capitalizing syllables.

Formatted text.

### Source
Reference to a resource from which the entry was collected or sourced. Examples include a specific dictionary or language researcher, or the places where the entry is used (in the case of dialectical variation, for example).

Plain text. 255 characters.

### Word Origin
Information about the history or etymology of the entry. Examples include the origin language of a borrowed word or the date the word came into the language.

Plain text. 255 characters.

### Contributor
A contributor is a person or group who aided in the making of the entry. While a contributor is usually a single person, it could also be a clan, tribe, culture group, or organization. A dictionary word can have multiple contributors. Examples include language speakers who recorded the word, or contributed knowledge and history of the word.
Names can be in any format that is appropriate for the content, eg: "John Smith" or "Smith, John."

Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.

## Word Entries
A dictionary word can have multiple word entries within it. This allows for more granular presentation of word conjugations, declensions, other forms (eg: gendered or plural forms), or display of closely connected forms of the word. Only the main word is shown when searching or browsing.

Each word entry can include all fields from the Mukurtu Essentials tab except cultural protocols, sharing setting, language, and glossary, since those describe the dictionary word as a whole. 

## Additional Fields

### Thumbnail
The thumbnail image is a clear visual example or illustration of the dictionary word. It is included in previews along with the term, translation, and recording fields.

ID, UUID, or title of the reference, title must be exact and match only one item.

### Media Assets
Additional media assets can further enrich a dictionary word. Examples include photos of a plant or animal named in the word, a longer video of the word being taught, or a relevant page from a language learning book. Supported media types are images, documents, video, audio, and embed code. Dictionary words can include more than one media asset, and each media asset can be a different media type. Media assets can be assigned a different cultural protocol from the dictionary word to allow differential access to the media assets and metadata.

IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.

### Keywords
Keywords are used to tag dictionary words to ensure that they are discoverable when searching or browsing.

Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.

### Map Points
A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a dictionary word. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools.

Note that this mapping data will be shared with the same users or visitors as the rest of the dictionary word. If the location is sensitive, carefully consider using this field.

geoJSON

### Location Description
A descriptive field to provide additional context and depth to the location(s) connected to the dictionary word.
Formatted text.

### Location (taxonomy)
A named place, or places, that are closely connected to the dictionary word. Examples include words that are place names,  where a word originated, or a place the word is otherwise connected to.

Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.

### Local Contexts
The Local Contexts Traditional Knowledge (TK) and Biocultural (BC) Labels are tools for Indigenous communities and local organizations. Developed through sustained partnership and testing within Indigenous communities across multiple countries, the Labels allow communities to express local and specific conditions for sharing and engaging in future research and relationships in ways that are consistent with already existing community rules, governance, and protocols for using, sharing, and circulating knowledge and data." For more information, visit <a href=https://localcontexts.org>localcontexts.org</a>.

#### Local Contexts Projects
This field will apply all of the Labels from the selected Local Contexts Project(s) to the dictionary word.

Local Contexts Project ID values, separated by your selected multi-value delimiter.

#### Local Contexts Labels and Notices
This field allows selective application of one or more Labels from any available Local Contexts Project to the dictionary word.

Local Contexts Project ID values, separated by your selected multi-value delimiter.

## Related Content

### Related Content
Dictionary words can be related to any other site content when there is a connection between those items that is important to show. Examples include digital heritage items that include the word.

IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.