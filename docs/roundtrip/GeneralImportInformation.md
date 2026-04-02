---
tags:
    - roundtrip
---

# General Import Information

!!! Roles "User roles" 
    Mukurtu manager, Roundtrip manager, Drupal administrator

## "Authored by" field

The authored by field can reference any valid username (create/edit access not required).
Regardless of author, protocols still apply to view and edit access.
The active user MUST have create/edit permissions in relevant protocols for all content in the sheet.



What happens when no author is assigned?

The active user is assigned as author.

This applies whether the "authored by" field is omitted or empty.

This also applies if the authored by field does not reference a valid username.

What happens when author is assigned and is different from active user, AND has correct permissions?

The username in "authored by" is correctly assigned.

What happens when author is assigned and is different from active user, AND has differing protocol roles?

Author has a permission that active user does not have?

Active user CANNOT complete the import, receives a community membership error.

Author does not have a permission that is required by protocols field, but active user does?

The named user is set as the author.

If content is created does the author have access that bypasses protocols?

They do not. Authorship does not seem to trump protocols.