---
tags:
    - roundtrip
---

# Using Export Lists

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

An export list lets you gather content over time into a named, reusable, and shareable group before exporting it, similar to a shopping cart. This article covers adding content to a list and managing your saved lists. See [Exporting Content](ExportingContent.md) for how to run an export from a list once it's ready.

## Add content to an export list

You can add items one at a time from a content page, or select multiple items at once while browsing.

### Add a single item

Start from either the content item itself, or a browse listing without opening it:

- Open the content item, then select "Add to export list".

    ![A digital heritage item's page, with the Add to export list button shown alongside View, Edit, Delete, and other actions.](../_embeds/exporting-content-node-actions-01.png)

- While browsing, select the "More actions" (**⋯**) menu next to an item, then choose "Add to export list".

    ![The More actions menu open for an item on the Browse Content page, with Add to export list listed alongside Edit, Add to Collection, and Export.](../_embeds/exporting-content-browse-more-actions-01.png)

Either way:

1. Under **Select an export list**, choose an existing list, or select "Create a new list..." and enter a **New list name**.
2. Select "Add to List".

![The Add to Export List form for a digital heritage item, with "Create a new list..." selected and a New list name field.](../_embeds/exporting-content-add-to-list-01.png)

!!! tip
    Depending on the item, you may see additional options here, such as including the other items in a collection or word list, related community records, an original record, or other pages of a multipage item. See [Exporting complex content](#exporting-complex-content) below for what these options do.

### Add multiple items

From your **Dashboard**, under **Content**, select **Manage Content**.

1. Select the checkbox next to each item you want to add.
2. Under **Action**, choose "Add to export list".
3. Select "Apply to selected items".

![The Action dropdown in the bulk operations bar set to "Add to export list", ready to apply to the 3 selected items.](../_embeds/exporting-content-manage-content-bulk-action-01.png)

You'll land on an Add to Export List page listing your selected items, where you choose an existing list under **Add to export list**, or enter a name under **Or create a new list**.

![The Add to Export List page for a bulk selection, listing the selected items with a Select export list dropdown and an Or create a new list field.](../_embeds/exporting-content-manage-content-add-to-list-01.png)

!!! tip
    Two toggles here apply to the whole selection: "Include all accessible community records for original records in this selection" and "Include all accessible pages for multipage items in this selection". See [Exporting complex content](#exporting-complex-content) below for what these include.

## Exporting complex content

Some content is made up of, or connected to, other content: a collection contains items, a word list contains words, an item can have community records built from an original record, and a multipage item is made up of individual pages. When you add one of these to an export list, or include it in an ad hoc export, Mukurtu offers additional options for how much of the connected content to bring along.

### Collections and word lists

When you add a collection or word list, select the checkbox to also include everything inside it:

- For a word list, this includes all of its words.
- For a collection, this includes the items directly in it. If the collection has sub-collections, a second checkbox lets you also include everything in those, recursively.

![The Add to Export List form for a collection, with both the "Include all items in this collection" and "Include all items in sub-collections" checkboxes checked.](../_embeds/exporting-complex-collection-01.png)

![The Add to Export List form for a word list, with the "Include all words in this word list" checkbox.](../_embeds/exporting-complex-wordlist-01.png)

### Community records and original records

Adding an original record offers three choices for its community records:

- **Just this record**: export only the original record.
- **This record and all accessible community records**: export the original record and every community record you can access.
- **This record and select community records**: choose which specific community records to include.

![The Add to Export List form for an original record, with the Community records radios: Just this record, This record and all accessible community records, and This record and select community records.](../_embeds/exporting-complex-communityrecords-01.png)

Adding a community record instead offers a single checkbox to also include the original record it's based on.

![The Add to Export List form for a community record, with the "Also include the original record" checkbox.](../_embeds/exporting-complex-originalrecord-01.png)

See [Understanding Community Records](../digital-heritage-items/UnderstandCommunityRecords.md) for more on how these relate to each other.

### Multipage items

Adding one page of a multipage item shows a checklist of every page in that item, all selected by default. Deselect any pages you don't want included.

![The Add to Export List form for a multipage item page, with a checklist of every page in the item, all checked.](../_embeds/exporting-complex-multipage-01.png)

See [Multipage Items](../digital-heritage-items/MultipageItems.md) for more on how these are structured.

## Manage your export lists

From your **Dashboard**, under **Roundtrip**, select **Export Lists**.

This page lists every export list you own or that's been shared with you, showing its **Name**, **Description**, number of **Items**, and **Visibility**. Select "Create new export list" to start a new one directly, or use the actions menu next to "Export" to edit or delete a list.

![The Export Lists page showing a list named First export list with 1 item and visibility set to Only You.](../_embeds/exporting-content-export-lists-01.png)

Editing a list lets you change its **Name** and **Description**, toggle **Share with all export users**, and remove items: select the checkbox next to each item to remove, then select "Remove selected".

![The Edit form for First export list, showing the Name and Description fields, the Share with all export users toggle, and the Content in this list table with a Remove selected button.](../_embeds/exporting-content-export-lists-edit-01.png)

