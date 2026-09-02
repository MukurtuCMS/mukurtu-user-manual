---
tags:
    - publication tools
    - comments
    - content
---

# Configuring Comments

!!! roles "User roles" 
    Mukurtu manager

Site-wide comment settings set the baseline for commenting across the whole site. For how these interact with per-protocol settings, see [Understanding Comments](UnderstandingComments.md).

## Access the site-wide comment settings

From your **Dashboard**, under **Publication Tools**, select **Site-wide comment settings**, or go directly to `/admin/config/mukurtu/commenting/settings`.

## Settings

### Site Wide Commenting

Enable or disable commenting for the entire site. When disabled, no content type can accept comments regardless of its own settings.

### Require Approval for Comments

When enabled, new comments are held for review and aren't visible to other users until approved. When disabled, comments publish immediately, unless a cultural protocol the content belongs to requires approval — a protocol's approval requirement always overrides this setting.

### Allow visitors to view comments

Allow visitors (users without an account) to read comments on content. This controls the *Access comments* permission for the Anonymous User role.

### Allow visitors to leave comments

Allow visitors to post comments. This option is only available when visitors are also allowed to view comments, and controls the *Post comments* permission for the Anonymous User role.

### Require email address from visitors who leave comments

When enabled, visitors must provide an email address to post a comment. The address is kept private and never shown publicly.

Select "Save configuration" when done.
