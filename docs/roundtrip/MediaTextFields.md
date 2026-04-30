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

!!! tip
    We do not recommend using the `<drupal-media data-entity-name="...">` or `<drupal-media data-entity-filename="...">` syntax unless full tag control is required.