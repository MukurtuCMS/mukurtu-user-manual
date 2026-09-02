---
tags:
    - publication tools
    - comments
    - content
---

# Understanding Comments

!!! roles "User roles" 
    Mukurtu manager, Protocol steward, Language steward, Authenticated users, Visitors

Mukurtu can let users leave comments on content, similar to a discussion thread below an item. Commenting can be turned on or off per content type, and who can see, post, and approve comments is controlled by two layers of settings working together.

## Two layers of settings

- **Site-wide settings** set the baseline for the whole site: whether commenting is on at all, whether comments require approval before they're visible, and whether visitors (people without an account) can view or post comments. See [Configuring Comments](ConfiguringComments.md).
- **Cultural protocol settings** let each protocol tighten those defaults for its own content. See the *Comment Settings* section of [Editing Cultural Protocol Settings](../communities-cultural-protocols-categories/EditCulturalProtocolSettings.md#comment-settings).

When an item belongs to multiple cultural protocols, or a protocol setting disagrees with the site-wide setting, the most restrictive option always wins. A protocol can require approval even if the site-wide setting doesn't, and can further restrict who may view or leave comments, but it can never loosen a restriction the site-wide settings or another one of the item's protocols already impose.

## Who can view and post comments

Viewing and posting comments are controlled separately. Authenticated users' access is managed through their user role's permissions. Visitors (anonymous users) are handled as a special case: a Mukurtu manager can allow or disallow visitors to view comments and, separately, to leave them, from the site-wide comment settings.

## Approval

When approval is required, a new comment isn't visible to other users until a reviewer approves it. See [Using Comments](UsingComments.md) for what a commenter sees when this happens, and [Reviewing Comments](ReviewingComments.md) for how a reviewer approves or removes a pending comment.
