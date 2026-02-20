---
tags:
    - roundtrip
    - media
---

# Importing New Media

!!! Roles "User roles" 
    TBD

## Prepare for import

- Prepare for import by collecting the media assets and metadata spreadsheets.
- Multiple media formats can be imported at the same time. Each media type will need it's own spreadsheet.
- See [Media Formats and Fields](MediaFormatsField.md) for information on preparing spreadsheets for import.

## Upload files 

1. From the dashboard, in the *Roundtrip* section, select *Import*. Or navigate directly to `/admin/import`.
2. In the *Metadata Files* field, select *Choose Files* to locate and upload the metadata spreadsheet(s).
3. In the *Media/Binary Files* field, select *Choose FIles* to locate and upload your local media files.
4. If necessary, files can be removed individually by selecting them with the toggle and selecting *Remove selected*.
5. The entire upload can be reset by selecting the additional actions menu and *Reset*.
6. When all files are uploaded, select *Next*.


## Configure and run import

- For each spreadsheet you will need to either select from an existing configuration, or create a new configuration.

1. Select the *Import Configuration* dropdown.
2. If you have already saved an import configuration and it is listed here, select the appropriate configuration.
3. If there is not an appropriate configuration listed, select *Customize Settings*.
    1. See [Managing Import Configurations](ManagingImportCOnfigurations.md) for more information.
4. Once all spreadsheets have the correct configuration selected, select *Review Import*. 
5. A list of all files will be provided. If it looks correct, select *Start Import*, otherwise select *Back* to make changes.
6. The importer will display progress, and when complete, a results page will display any success and error messages, as well as a list of all imported media.
7. To return to the main import page and reset the import files, select *Start a new import*.