---
tags:
    - roundtrip
---

# General Import Information

!!! Roles "User roles" 
    Mukurtu manager, Roundtrip manager, Drupal administrator

## "Authored by" field

All import sheets can include an optional `Authored by` field. This is used to indicate which user is responsible for creating the imported content. It can be useful to identify content authors and to track the revision history of content as it is changed.

- The `Authored by` field can reference any valid username.
- The user running the import MUST have correct protocol permissions for all content and protocols referenced in the sheet.
- If a user is listed as the author of content and later loses permission to access the content due to protocol membership changes, then they cannot access the content. Being the author of content does not bypass over override protocol access controls.

**If no author is provided** (if the field is empty, omitted entirely, or does not reference a valid username)

- The user running the import is listed as the author.

**If an author with correct protocol permissions is provided, AND the user running the import has correct protocol permissions**

- The user identified in the `Authored by` field is listed as the author.

**If an author with correct protocol permissions is provided, BUT the user running the import does NOT have correct protocol permissions**

- The import will fail with a community membership error. The user running the import MUST have correct protocol permissions.

**If an author with INCORRECT protocol permissions is provided, BUT the user running the import DOES have correct protocol permissions**

- The user running the import is listed as the author.










