---
tags: 
    - roundtrip
    - content
    - metadata
---
# Embedding media in formatted text fields

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

Users can include media assets in formatted text fields such as the Description or Location description fields using the following syntax. The syntax are presented in order of our recommended methods. 

|Syntax|Lookup|Attributes|
|---|---|---|
|`{{media:My Image}}` or `{{media:photo.jpg}}`|Name, then filename fallback|Default view mode|
|`[media name="My Image"]`|Name only|view-mode, align, caption, alt|
|`[media filename="photo.jpg"]`|Filename only|view-mode, align, caption, alt|
|`<drupal-media data-entity-name="...">`|Name only|Full tag control|
|`<drupal-media data-entity-filename="...">`|Filename only|Full tag control|

## {{media:My Image}} or {{media:photo.jpg}}

This syntax is recommended and is going to work in almost all cases. Use this unless you know you need specific alignment, captioning, embed size, or full tag control.

## [media name="My Image"] or [media filename="photo.jpg"]

Use this syntax if you know that you are going to need more control over alignment, captioning, embed size, or full tag control.

Tags can be added to the syntax to specify alignment, add captioning, or adjust the embed size. A full list of these tags can be found at [ckeditor.com](https://ckeditor.com/docs/ckeditor5/latest/features/html/general-html-support.html#block-elements).

We do not recommend using the `<drupal-media data-entity-name="...">` or `<drupal-media data-entity-filename="...">` syntax unless full tag control is required.