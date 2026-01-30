---
tags:
    - roundtrip
---

# Export Settings

!!! Roles "User roles" 
    TBD

- Users can configure different export settings for easy re-use. 
- This is found at `/admin/export/settings`
- This is included because as shown in the overview there are many different use cases for Roundtrip. For example I may want different export settings for:
    - Exporting so I can made edits and import/update my own site.
    - Exporting to another community with their own Mukurtu site.
    - Exporting certain fields of content to send to an outside institution.
    - Exporting metadata only, or with media assets included.
- We have packaged a basic "recommended settings for import" settings for in-site updates, but would like to include a few other useful pre-sets if we can define them.

## Adding a CSV export setting

- A new export setting can be created at `/admin/export/format/csv/add` (or from dashboard/export links.)
- Configuration options include, but may not be limited to...
    - Granular per-content/media/etc per field selection/omission.
    - Per-field header changes.
    - Use of either IDs or UUIDs.
    - Media references or binary files.
    - Bare content or included references.
    - CSV settings (delimiter, escape character, etc)
