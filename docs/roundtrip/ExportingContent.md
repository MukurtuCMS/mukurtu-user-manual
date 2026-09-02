---
tags:
    - roundtrip
---

# Exporting Content

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

There are two ways to export content. An export list lets you gather items over time into a named, reusable, and shareable group before exporting them. An ad hoc export skips that step and exports one or more items right away. Either way, the export itself uses an export setting that controls exactly which fields are included. This article covers both approaches. For how to configure what an export includes, see [Export Settings](ExportSettings.md).

!!! requirement
    Users must be an Administrator, Mukurtu manager, or Roundtrip manager to access export tools. See [Manage User from a Site-wide role](../users/manage-user-accounts-site-wide.md) for more information.

## Add content to an export list

Content is gathered into a named export list before you export it, similar to a shopping cart. You can add items one at a time from a content page, or select multiple items at once while browsing.

### Add a single item

1. Open the content item you want to export.
2. Select "Add to Export List".
3. Under *Select an export list*, choose an existing list, or select "Create a new list..." and enter a *New list name*.
4. Select "Add to List".

![The Add to Export List form for a digital heritage item, with "Create a new list..." selected and a New list name field.](../_embeds/exporting-content-add-to-list-01.png)

!!! tip
    Depending on the item, you may see additional options here, such as including the other items in a collection or word list, related community records, an original record, or other pages of a multipage item. See [Exporting Complex Content](ExportingComplexContent.md) for what these options do.

### Add multiple items

While browsing or searching content, select the items you want, then choose "Add to Export List" from the bulk actions menu.

## Manage your export lists

From your **Dashboard**, under **Roundtrip**, select **Export Lists**.

This page lists every export list you own or that's been shared with you, showing its *Name*, *Description*, number of *Items*, and *Visibility*. Select "Create new export list" to start a new one directly, or use the actions menu next to a list to edit or delete it.

![The Export Lists page showing a list named Sample export with 2 items and visibility set to Only You.](../_embeds/exporting-content-export-lists-01.png)

!!! tip
    Setting a list's visibility to "All Export Users" shares it with other users who have export access. Otherwise it's visible to "Only You".

## Run an ad hoc export

An ad hoc export skips export lists entirely: you export one or more items right away, without saving them anywhere first. Use this when you just need a one-off export and don't need to reuse or share the selection later.

- From a single content item, select "Export" instead of "Add to Export List".
- While browsing or searching content, select the items you want, then choose "Export" from the bulk actions menu instead of "Add to Export List".

Either way, you'll land on the same export page described below, except instead of an *Export list* dropdown you'll see a summary of the items you selected.

!!! tip
    Select "Clear Selection" on the export page to start over with a different ad hoc selection.

## Run an export from a list

There are two ways to start an export from a saved list:

- From **Export Lists**, select "Export" next to the list you want to export.
- From your **Dashboard**, under **Roundtrip**, select **Export Settings**, then choose a list from the *Export list* dropdown.

Either way, you'll land on the same export page. From here:

1. Under *Export Settings*, choose which saved CSV export setting to use for this export. See [Export Settings](ExportSettings.md) for what these control. If you don't have one yet, select "New CSV export setting" to create one.
2. If your list or ad hoc selection includes a collection, word list, original record, community record, or multipage item, you may see additional options here for how much connected content to include. See [Exporting Complex Content](ExportingComplexContent.md) for what these options do.
3. Select "Start Export".

![The export page with a list selected under Export list, a saved CSV export setting selected under Export Settings, and the Start Export button.](../_embeds/exporting-content-run-export-01.png)

## Download your export

Once the export finishes, the Export Results page lists how many items of each type were exported and provides a "Download Export" link. Select "Back to Settings" to run another export with the same list, or "New Export" to start over with a different one.

![The Export Results page showing 2 content items exported and a Download Export link.](../_embeds/exporting-content-results-01.png)
