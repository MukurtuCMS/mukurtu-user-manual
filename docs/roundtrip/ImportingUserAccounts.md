---
tags:
    - roundtrip
    - users
---

# Importing User Accounts

!!! roles "User roles"
    Administrator

User accounts can be created and updated in bulk the same way as content, through the regular import wizard. See [Importing Content](ImportingContent.md) for the general steps.

!!! requirement
    Importing user accounts requires the separate *Import User Accounts* permission, in addition to general roundtrip access. This permission is restricted and isn't granted to the Mukurtu manager or Roundtrip manager roles by default.

## Choose the user import type

When configuring your import, select **User** as the import type.

## Fields

- *Username*, *Email*, *Display Name*: standard account fields.
- *Account Status*: one of *Active*, *Blocked*, or *Pending* (case-insensitive). Leave blank to default new accounts to Active; updated accounts keep their current status if left blank.
- *Roles*: the roles this user should have, by label (e.g. "Community Manager") or machine name (e.g. `community_manager`). Every user automatically gets the Authenticated user role; you don't need to include it.
- *Communities* and *Protocols*: the communities and protocols this user is a member of, and their role in each. Format: `CommunityName>role|role;AnotherCommunity>role`, separating multiple roles for the same group with `|` and multiple groups with your configured multi-value delimiter.
- *ID*, *UUID*: to update an existing account.

!!! warning
    Passwords are never importable. There's no field for one, and no plaintext password is ever read from or written to an import file.

!!! requirement
    The Administrator role can never be assigned through an import, and the site's original superuser account can never be created or updated this way, regardless of who runs the import.

## Community and protocol membership

Granting a user membership in a community or protocol through an import requires the same "manage members" access you'd need to add that member manually. This is checked per group named in the *Communities*/*Protocols* columns, not just your general import permission, so a community or protocol's own stewards keep control over their own membership regardless of who else can run user imports.

## Send account setup emails

On the review step, select the "Send account setup emails to newly created users" checkbox to email each newly created account with an email address the standard "set your password" link. Existing accounts that are updated never receive this email.

## Results

User imports don't have a detailed per-row results list. Instead, the results page shows a simple count of accounts created, updated, and failed. For the full history of past import runs, see [Import Logs](ImportLogs.md).
