---
tags:
    - roundtrip
---

# Importing Content

!!! Roles "User roles" 
    Administrator, Mukurtu manager, Roundtrip manager

In Mukurtu 3, there were many different starting points for import, depending on the content type or media being imported, or if importing multiple content types/media.

Metadata of a single content type went straight to an upload form with no configuration options, and multiple components required quite complex interrelated spreadsheets and media files properly arranged in zipped folders.

Now there is a more flexible single import start point that can handle more complexity.

This article will walk you through the general steps to import a .csv metadata sheet and accompanying media assets. While the basic steps are the same for each content type, there are differences between them that will not be detailed here. Please refer to the import article for the content type you are importing for more detail:

- [Import Digital Heritage Items](../roundtrip/DHItems.md) 
- [Import Dictionary Words](../roundtrip/Dictionary.md)
- [Import Person records](../roundtrip/PersonRecords.md)
- [Import Place Records](../roundtrip/PlaceRecords.md)
- [Import Word Lists](../roundtrip/WordLists.md)
- [Import Collections](../roundtrip/Collections.md)
- [Import Media](../roundtrip/ImportingNewMedia.md)

!!!Requirement 
    Users must either be a Mukurtu manager or a Mukurtu Roundtrip manager to access roundtrip tools. Mukurtu roundtrip managers will only be able to upload according to their protocol permissions. See [Manage User from a Site-wide role](../users/manage-user-accounts-site-wide.md) for more information.

## Upload content

To import content, go to `/admin/import` or from the dashboard, select **Import**.

![The dashboard with the import link highlighted.](../_embeds/import-content-01.png)

The import page has two upload fields. The first field is for .csv sheets only. The second field is for media or binary files that are referenced in the spreadsheet. You can upload multiple files in each field. 

!!! Requirement
    To upload media, you must upload an accompanying metadata sheet that references the media file.

1. Under **metadata files** select "choose files." Select the file(s) you would like to upload.  
2. Under **media/binary files** select "choose files." Select the media file(s) you woud like to upload.

Any combination of CSV sheets and supported media assets can be selected. Successfully selected files should be listed below the appropriate field. When you are done, select "Next" to continue on to the file configuration page.

![The import page showing one csv spreadsheet and 3 media assets selected for upload](../_embeds/import-content-02.png)


### Configure import settings

The file configuration page lists each spreadsheet you've uploaded. If your sheet's columns map to a custom configuration you have already saved, that saved configuration will be available in the import configuration drop-down menu. If not, select "customize settings" to map your spreadsheet onto the appropriate metadata fields for the content item.

![The file configuration page showing the spreadsheet file name, the import configuration drop down menu and the customize settings button](../_embeds/import-content-03.png)

#### Import type

1. There are several types of imports. In this case, we are importing content. Select **content**. 

    - This is a required field.

2. Under *import sub-type*, select a sub-type. Because the import type is content, all content types will be listed here. If the import type was media, the sub-type would list all media types, etc. The fields used for mapping will be determined by the type and sub-type selections. 

![The import type is content and the sub-type is digital heritage item. Both are selected for import type and sub-type](../_embeds/import-content-18.png)

#### Define custom source/target mappings
The column headers in your metadata sheet do not need to match Mukurtu's metadata schema. This next section allows you to map your column headers to Mukurtu. On the left you will see your spreadsheet's column names. To the right are the Mukurtu target fields. Each dropdown menu in the target fields column lists all metadata fields for the content type you are uploading.

Column names that match Mukurtu's metadata schema will map automatically (title and description fields for example). You can select a different field if desired. 

![Column names match Mukurtu's metadata schema and are automatically mapped](../_embeds/import-content-06.png)

Column names that Mukurtu does not recognize will be labeled "Ignore - Do not Import." 

![Column names that do not match Mukurtu's metadata schema. "Ignore - Do not Import." is auto-selected in the target fields column](../_embeds/import-content-07.png)

For each column name you wish to map, open the corresponding menu and select the appropriate Mukurtu metadata field.

![Mapping the protocol field to Cultural Protocols > Protocols](../_embeds/import-content-08.png)

![The protocol column is now mapped correctly to Cultural Protocols > Protocols](../_embeds/import-content-09.png)

!!! Tip
    Note that you cannot map two columns to the same field. For example, if you have two columns labeled "source," you cannot select "source" twice as a target field.

#### File settings
When your mapping is complete, scroll down to file settings and ensure that the default settings reflect your spreadsheet. Make any necessary changes to ensure your spreadsheet is read correctly.

![The default file settings](../_embeds/import-content-11.png)

#### Import configuration template
If you will be uploading other sheets that match these settings, you can save this as a template for future uploads, and these configuration steps won't have to be repeated.

To save a template, set the toggle to green and give your template a descriptive title. When you are done, select "Save." You will be returned to the file configuration page. 

![Saving a template by setting the toggle to green and adding a template name](../_embeds/import-content-10.png)


### Review and run import
If you saved your template, you will now see it selected in the import configuration dropdown menu with a summary of the content type, number of fields mapped, and number of fields ignored. If you need to make additional changes, select "Customize Settings" to return to the import settings. When you are ready to proceed with the import, select "Review Import."

![The updated file configuration page showing count of mapped fields and the newly saved template](../_embeds/import-content-12.png)

The import review page lists all included metadata, media files and configurations. If everything looks correct, select "Start Import."

![The import review page listing metadata and media files. The start import button is highligted.](../_embeds/import-content-13.png)

The import will run. When complete, a results page will populate with a success message and a list of items that imported successfully. Select the titles to view each item.

![The results page with a success message and list of imported items](../_embeds/import-content-14.png)

## Upload paragraphs
Most content types include paragraphs, which is a bundle of metadata within a content item that is uploaded in a separate spreadsheet. Each metadata bundle is assigned an ID that is referenced in the base content sheet. 

Content items and their paragraphs can be uploaded together. In this example, DH items are being uploaded with a Citing Indigenous Elders and Knowledge Keepers Paragraph. 

![The upload files page showing a DH item csv and paragraph csv in that order](../_embeds/import-content-15.png)

!!! Requirement
    The base content item must be selected before the paragraph so that the system can reference it as the paragraph is imported.

On the file configuration page, you will see two sheets that need to be configured. Follow the [configure import settings](#configure-import-settings) steps for each sheet.

When configuring the paragraph sheet, select **compound types** as the import type, and the appropriate paragraph type as your sub-type.

![The import type and subtype. Compound type and Citing Indigenous Elders and Knowledge Keepers are selected](../_embeds/import-content-16.png)

### Identifier Column
Select the column in your sheet that will serve as the *identifier column*. This tells the system where the word entry IDs are located so that they can be paired with the correct content item.

![The ID column is selected in the identifier column field](../_embeds/import-content-19.png)

In this example of a dictionary word and word entry, the ID of the word entry is referenced in the dictionary word. When uploading the word entry sheet, the identifier column should be set to "ID". 

![Sample dictionary word spreadsheet showing a term and word entry field. The word entry field is populated with an ID](../_embeds/import-content-04.png)

Continue with the mapping and import by following the steps in [Review and run import](#review-and-run-import)


