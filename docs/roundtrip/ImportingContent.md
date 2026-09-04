---
tags:
    - roundtrip
---

# Importing Content Overview

!!! roles "User roles" 
    Administrator, Mukurtu manager, Roundtrip manager

This article will walk you through the general steps to import a .csv metadata sheet and accompanying media assets. While the basic steps are the same for each content type, there are specifics about each type that are discussed in dedicated articles. Please refer to the article for the content type you are importing for more detail.

## Upload content

To import content, go to `/admin/import` or from the dashboard, select **Import**.

![The dashboard with the import link highlighted.](../_embeds/import-content-01.png)

The import page has two upload fields. The **metadata files** field is for .csv sheets only. The **media/binary files** field is for media or binary files that are referenced in the csv sheets. You can upload multiple files in each field. 

!!! requirement
    To upload media, you must upload an accompanying metadata sheet for the media asset that is separate from the content item. See [Importing Media Assets](../roundtrip/MediaFormatsFields.md) for instructions.

1. Under **metadata files** select "choose files." Select the file(s) you would like to upload. 

2. Under **media/binary files** select "choose files." Select the media file(s) you would like to upload.

Any combination of CSV sheets and supported media assets can be selected. When you are done, select "Next" to continue on to the file configuration page.

![The import page showing two csv spreadsheets and 2 media assets selected for upload](../_embeds/import-content-02.png)

## Choose an import template

Once your files are uploaded, you need to select your desired import mapping. You can select an existing import template, and if needed, modify it or create a new one. See [Import Templates](ImportTemplates.md) for the full walkthrough, including saving your mapping as a reusable template.

![The file configuration page showing the spreadsheet file name, the import configuration drop down menu and the customize settings button](../_embeds/import-content-03.png)

## Review and run import
If you saved your template, you will now see it selected in the import configuration dropdown menu with a summary of the content type, number of fields mapped, and number of fields ignored. If you need to make additional changes, select "Customize Settings" to return to the import template. When you are ready to proceed with the import, select "Review Import."

![The updated file configuration page showing count of mapped fields and the newly saved template](../_embeds/import-content-12.png)

The import review page lists all included metadata, media files and configurations. If everything looks correct, select "Start Import."

![The import review page listing metadata and media files. The start import button is highlighted.](../_embeds/import-content-13.png)

The import will run. When complete, a results page will populate with a success message and a list of items that imported successfully. Select the titles to view each item.

![The results page with a success message and list of imported items](../_embeds/import-content-14.png)

This results page is only available right after the import runs. For a permanent history of every import you've run, see [Import Logs](ImportLogs.md).

