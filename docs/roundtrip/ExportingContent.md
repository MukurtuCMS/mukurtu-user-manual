---
tags:
    - roundtrip
---

# Exporting Content

!!! roles "User roles"
    Administrator, Mukurtu manager, Roundtrip manager

There are three ways to export content:

1. An export list lets you gather items over time into a named, reusable, and shareable group before exporting them.
2. An on the fly export directly from a content page which bypasses export lists and runs an export right away. 
3. An on the fly export from the manage content view (`/admin/content`) which bypasses export lists and runs an export right away.

## Run an export from a list

There are two ways to start an export from a saved list:

- From your **Dashboard**, under **Roundtrip**, select **Export Lists**, select "Export" next to the list you want to export. See [Using Export Lists](UsingExportLists.md) for how to build and manage your lists.
- From your **Dashboard**, under **Roundtrip**, select **Export Settings**, then choose a list from the *Export list* dropdown.

Either way, you'll land on the same export page. From here:

1. Under *Export Settings*, choose which saved CSV export setting to use for this export. See [Export Settings](ExportSettings.md) for what these control. If you don't have one yet, select "New CSV export setting" to create one.
2. If your list or on the fly selection includes a collection, word list, original record, community record, or multipage item, you may see additional options here for how much connected content to include. See [Exporting complex content](UsingExportLists.md#exporting-complex-content) for what these options do.
3. Select "Start Export".

    ![The export page with a list selected under Export list, a saved CSV export setting selected under Export Settings, and the Start Export button.](../_embeds/exporting-content-run-export-01.png)

4. Wait for the export to finish.

    ![The Exporting progress screen with a progress bar and "Initializing export" status.](../_embeds/exporting-content-progress-01.png)

5. The Export Results page lists how many items of each type were exported. Select "Download Export" to download the file. Select "Back to Settings" to run another export with the same list, or "New Export" to start over with a different one.

    ![The Export Results page showing 2 content items exported and a Download Export link.](../_embeds/exporting-content-results-01.png)

## Run an on the fly export from a content page

An on the fly export skips export lists entirely and you can export an item right away, without saving it to an export list. Use this when you just need a one-off export and don't need to reuse or share the selection later.

Start from either the content item itself, or a browse listing without opening it:

- Open the content item, then select "Export" instead of "Add to Export List".

    ![A digital heritage item's page, with the Export button shown alongside View, Edit, Delete, and other actions.](../_embeds/exporting-content-node-actions-01.png)

- While browsing, select the "More actions" (**⋯**) menu next to an item, then choose "Export" instead of "Add to export list".

    ![The More actions menu open for an item on the Browse Content page, with Export listed alongside Edit, Add to Collection, and Add to export list.](../_embeds/exporting-content-browse-more-actions-01.png)

Either way, you'll land on the same export page described above, except instead of an *Export list* dropdown you'll see a summary of the item you selected.

!!! tip
    Select "Clear Selection" on the export page to start over with a different on the fly selection.

Select "Start Export", then wait for the export to finish. The Export Results page lists how many items of each type were exported. Select "Download Export" to download the file. Select "Back to Settings" to run another export, or "New Export" to start over with a different selection.

![The Exporting progress screen with a progress bar and "Initializing export" status.](../_embeds/exporting-content-progress-01.png)

![The Export Results page showing 2 content items exported and a Download Export link.](../_embeds/exporting-content-results-01.png)

## Run an on the fly export from Manage Content

An on the fly export from Manage Content lets you export several items at once without saving them to an export list first.

From your **Dashboard**, under **Content**, select **Manage Content**. Select the checkbox next to each item you want, choose "Export" under **Action**, then select "Apply to selected items".

![Three items selected in Manage Content, with "Export" chosen in the bulk Action dropdown.](../_embeds/exporting-content-manage-content-export-01.png)

You'll land on the same export page described above, except instead of an *Export list* dropdown you'll see a summary of the items you selected.

!!! tip
    Select "Clear Selection" on the export page to start over with a different on the fly selection.

Select "Start Export", then wait for the export to finish. The Export Results page lists how many items of each type were exported. Select "Download Export" to download the file. Select "Back to Settings" to run another export, or "New Export" to start over with a different selection.

![The Exporting progress screen with a progress bar and "Initializing export" status.](../_embeds/exporting-content-progress-01.png)

![The Export Results page showing 2 content items exported and a Download Export link.](../_embeds/exporting-content-results-01.png)
