---
tags: 
    - migration
---

# Exporting Site Data from Reclaim Hosting

To move a Mukurtu 3 site from Reclaim Hosting to another hosting provider, you will need to export the database and the public and private files. 

!!! Note
    If you are using Mukurtu 3 now, and plan to migrate to Mukurtu 4, you should complete the [pre-migration activities](PM02Activities.md) NOW so that you can migrate directly into a new Mukurtu 4 instance. Otherwise you may need to setup Mukurtu 3 on your new hosting provider and then migrate to Mukurtu 4 later.

## Export the database

1) Determine which database you need to export by logging into Reclaim, accessing the cPanel and then selecting “My Apps”.

![Reclaim client portal](../_embeds/DBExport01.png)

![Reclaim cPanel](../_embeds/DBExport02.png)

2) Find your Mukurtu instance and select "Edit".

![Reclaim MyApps](../_embeds/DBExport03.png)

3) Select the settings tab, then "Databases" and note the *Database Name*.

![Reclaim database names](../_embeds/DBExport04.png)

4) Return to the main cPanel menu and find the *Databases section* and select “phpMyAdmin”.

![Reclaim cPanel](../_embeds/DBExport05.png)

5) In phpMyAdmin, find and select the database name from step 3, select the “export” tab, and "Export Method > Custom".

![Reclaim phpMyAdmin](../_embeds/DBExport06.png)

6) Locate the "Object creation options” settings and ensure that “Add DROP TABLE [....]" setting is on.

![Reclaim phpMyAdmin](../_embeds/DBExport07.png)

7) Scroll to the end of the page and select “Export”.

8) The file will download with a “.sql” extension. This may take a few minutes to complete.

![file download](../_embeds/DBExport08.png)

These files can be quite large, to optimize sharing it is a good idea to compress the file:

    - On a Mac, right-click and select “compress”.
    - On Windows, right-click and select “send to” > Compressed (Zipped) Folder. 

 ![finder file compression](../_embeds/DBExport09.png)

## Download a backup of the site files

1) While logged into your Reclaim account, access the cPanel and then select “My Apps”.

![finder file compression](../_embeds/BackupExport01.png)

2) Find your Mukurtu instance and select "Backup". We strongly recommend creating a new backup now.

![finder file compression](../_embeds/BackupExport02.png)

3) Provide an identifiable name for the backup and select "-> Backup". 

![finder file compression](../_embeds/BackupExport03.png)

4) A progress bar will be displayed. This may take a few minutes to complete.

![finder file compression](../_embeds/BackupExport04.png)

5) When the backup is complete, select "My Backups" at the top of the page.

![finder file compression](../_embeds/BackupExport05.png)

6) Locate the backup you just created and select the "options" icon, then select "Download".

![finder file compression](../_embeds/BackupExport06.png)

The file will download with a “.tar.gz” extension. This may take a few minutes to complete.

![finder file compression](../_embeds/BackupExport07.png)
