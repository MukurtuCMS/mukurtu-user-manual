---
tags: 
    - roundtrip
    - content
    - metadata
    - dictionary
---
# Importing Dictionary Words

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Import templates can be created and downloaded from your own site at `/admin/import/format` (linked on the dashboard as "Import format information"). For more information on dictionary word metadata fields, refer to [Dictionary Word Metadata](../dictionary/DictionaryWordMetadata.md)

## Dictionary words

|Field Name|Description|Format Information|
|---|---|---|
|**Required**|**Cannot be empty**||
|Term|A word, term, phrase, or other language element.|This field is plain text and limited to 255 characters.|
|Cultural Protocols > Protocols||IDs, UUIDs, or names of the cultural protocols, separated by your selected multi-value delimiter. If using names, they must be exact and match only a single protocol.|
|Cultural Protocols > Sharing Setting||Either 'Any' or 'All', case insensitive.|
|Language|Each dictionary word is associated with one language. Dictionary languages must first be configured by a Mukurtu Manager.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary.|
|ID|Only used when updating existing dictionary words, not when creating new dictionary words.|Integer.|
|**Required**|**Will autofill if empty**||
|UUID|A UUID will be generated on import.|UUID (e.g., 6b77cc9e-5fdf-4750-891e-e705b7bf323b) value.|
|**Mukurtu Essentials**|
|Glossary Entry|By default, the dictionary word will be indexed, sorted, or alphabetized by the first character of the term if this field is not included. The glossary entry is used for indexing when a character or letter other than the first character in the term should be referenced. Examples include diacritic or accent-initial words, root word markers at the start of the term, or combined characters (eg: ch or á in some languages are considered a single character).|This field is plain text and limited to 255 characters.|
|Alternate Spelling|An alternate spelling of the term. Examples include historic or current variant spellings, spellings from different dialects or in different writing systems, or any other alternate spelling that will help find the dictionary word when searching.|This field is plain text and limited to 255 characters.|
|Translation|Translations of the entry into other languages. Consider indicating the language of the translation, eg: Apple (English).|This field is plain text and limited to 255 characters, separated by your selected multi-value delimiter.|
|Recording|Audio recordings of the entry being spoken, usually on its own. Multiple recordings may be used to represent different types of speakers (eg: speakers of different ages, genders, accents, or dialects), or different forms the entry can take. Recordings can be assigned a different cultural protocol from the dictionary word to allow differential access to the recordings and metadata.|ID, UUID, or title of the reference. The title must be exact and match only one item.|
|Definition|A longer definition or description of the entry.|Formatted text.|
|Sample Sentences|The sample sentence and recording fields are repeatable. They can be bundled together (text and corresponding recording) or used separately (just text or just a recording). See [Word entries and sample sentences](#word-entries-and-sample-sentences) for more information.|The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Word Type|Word types may include parts of speech, syntactic or grammatical categories, or any other relevant system to classify entries.|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Pronunciation|A pronunciation guide used to teach language learners the correct pronunciation of the entry. Pronunciation guides may use a standard phonetic alphabet or whatever notation system is used by speakers and teachers of the language, eg: indicating stress with bold text or capitalizing syllables.|Formatted text.|
|Source|Reference to a resource from which the entry was collected or sourced. Examples include a specific dictionary or language researcher, or the places where the entry is used (in the case of dialectical variation, for example).|This field is plain text and limited to 255 characters.|
|Word Origin|Information about the history or etymology of the entry. Examples include the origin language of a borrowed word or the date the word came into the language.|This field is plain text and limited to 255 characters.|
|Contributor|A contributor is a person or group who aided in the making of the entry. While a contributor is usually a single person, it could also be a clan, tribe, culture group, or organization. A dictionary word can have multiple contributors. Examples include language speakers who recorded the word, or contributed knowledge and history of the word. Names can be in any format that is appropriate for the content, eg: "John Smith" or "Smith, John."|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|**Word Entries**|
|Word Entry|A dictionary word can have multiple word entries within it. This allows for more granular presentation of word conjugations, declensions, other forms (eg: gendered or plural forms), or display of closely connected forms of the word. See [Word entries and sample sentences](#word-entries-and-sample-sentences) for more information.|The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|**Additional Fields**|
|Thumbnail|The thumbnail image is a clear visual example or illustration of the dictionary word. It is included in previews along with the term, translation, and recording fields.|ID, UUID, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Media assets|Additional media assets can further enrich a dictionary word. Examples include photos of a plant or animal named in the word, a longer video of the word being taught, or a relevant page from a language learning book. Supported media types are images, documents, video, audio, and embed code. Dictionary words can include more than one media asset, and each media asset can be a different media type. Media assets can be assigned a different cultural protocol from the dictionary word to allow differential access to the media assets and metadata.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|
|Keywords|Keywords are used to tag dictionary words to ensure that they are discoverable when searching or browsing.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Map points|A detailed, interactive mapping tool that allows placing and drawing multiple locations related to a dictionary word. Locations can be single points, paths, rectangles, or free-form polygons. Each location can be given a basic label. This field is also used for the browse by map tools.|GeoJSON data format.|
|Location description|A descriptive field to provide additional context and depth to the location(s) connected to the dictionary word.|Formatted text.|
|Location (taxonomy)|A named place, or places, that are closely connected to the dictionary word. Examples include words that are place names, where a word originated, or a place the word is otherwise connected to.|Taxonomy term names, IDs, or UUIDs, separated by your selected multi-value delimiter. Each name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Local Contexts Projects|This field will apply all of the Labels from the selected Local Contexts Project(s) to the dictionary word.|Project titles or IDs, separated by your selected multi-value delimiter.|
|Local Contexts Labels and Notices|This field allows selective application of one or more Labels from any available Local Contexts Project to the dictionary word.|Label or notice names, separated by your selected multi-value delimiter.|
|**Related Content**|
|Related content|Dictionary words can be related to any other site content when there is a connection between those items that is important to show. Examples include digital heritage items that include the word.|IDs, UUIDs, or titles of the references, separated by your selected multi-value delimiter. Each title must be exact and match only one item.|

## Word entries and sample sentences

Word entries and sample sentences are groups of repeatable fields that are handled as "paragraphs" in import. To include sample sentences or word entries in a dictionary word, you will need to include a corresponding spreadsheet as well. Those spreadsheets are included in this article, but please review [General Import Information > Importing Paragraphs](./GeneralImportInformation.md#paragraphs) for more information on how to format and connect the spreadsheets during an import.

- If including **Sample Sentences** and **Word Entries**, the Dictionary Word CSV and associated paragraph CSVs must be given unique IDs. Those IDs do not have to be uploaded, but are what you will use to tie the paragraphs to the proper dictionary word. 
- You can use the same CSV for sample sentences that are in the main entry and in word entries. To do this, ensure they are connected properly via an ID.

### Sample Sentences

|Field Name|Description|Format Information|
|---|---|---|
|Import ID, ID, or UUID|When importing a dictionary word and corresponding sample sentences at the same time, use an *Import ID*|See [General Import Information > Identifiers](./GeneralImportInformation.md#identifiers-name-id-uuid-import-id) for more information.|
|Sample Sentence|Text entry of the sample sentence|This field is plain text and limited to 255 characters.|
|Recording|Audio recording of the sample sentence.|ID, UUID, or title of the reference. The title must be exact and match only one item.|

### Word Entries

|Field Name|Description|Format Information|
|---|---|---|
|Import ID, ID, or UUID|When importing a dictionary word and corresponding sample sentences at the same time, use an *Import ID*|See [General Import Information > Identifiers](./GeneralImportInformation.md#identifiers-name-id-uuid-import-id)
|Term|A word, term, phrase, or other language element.|This field is plain text and limited to 255 characters.|
|Alternate Spelling|An alternate spelling of the term. Examples include historic or current variant spellings, spellings from different dialects or in different writing systems, or any other alternate spelling that will help find the dictionary word when searching.|This field is plain text and limited to 255 characters.|
|Translation|Translations of the entry into other languages. Consider indicating the language of the translation, eg: Apple (English).|This field is plain text and limited to 255 characters, separated by your selected multi-value delimiter.|
|Recording|Audio recordings of the entry being spoken, usually on its own. Multiple recordings may be used to represent different types of speakers (eg: speakers of different ages, genders, accents, or dialects), or different forms the entry can take. Recordings can be assigned a different cultural protocol from the dictionary word to allow differential access to the recordings and metadata.|ID, UUID, or title of the reference. The title must be exact and match only one item.|
|Definition|A longer definition or description of the entry.|Formatted text.|
|Sample Sentences|The sample sentence and recording fields are repeatable. They can be bundled together (text and corresponding recording) or used separately (just text or just a recording). See [Word entries and sample sentences](#word-entries-and-sample-sentences)for more information.|The ID or UUIDs of the paragraphs, separated by your selected multi-value delimiter.|
|Word Type|Word types may include parts of speech, syntactic or grammatical categories, or any other relevant system to classify entries.|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
|Pronunciation|A pronunciation guide used to teach language learners the correct pronunciation of the entry. Pronunciation guides may use a standard phonetic alphabet or whatever notation system is used by speakers and teachers of the language, eg: indicating stress with bold text or capitalizing syllables.|Formatted text.|
|Source|Reference to a resource from which the entry was collected or sourced. Examples include a specific dictionary or language researcher, or the places where the entry is used (in the case of dialectical variation, for example).|This field is plain text and limited to 255 characters.|
|Word Origin|Information about the history or etymology of the entry. Examples include the origin language of a borrowed word or the date the word came into the language.|This field is plain text and limited to 255 characters.|
|Contributor|A contributor is a person or group who aided in the making of the entry. While a contributor is usually a single person, it could also be a clan, tribe, culture group, or organization. A dictionary word can have multiple contributors. Examples include language speakers who recorded the word, or contributed knowledge and history of the word. Names can be in any format that is appropriate for the content, eg: "John Smith" or "Smith, John."|Taxonomy term name, ID, or UUID. The name must be exact and match only one term in that vocabulary. New terms will be created if they do not already exist.|
