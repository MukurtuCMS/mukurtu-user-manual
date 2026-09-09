---
tags: 
    - migration
---

# Running the Mukurtu 3 to Mukurtu 4 Migration

!!! warning
    This documentation assumes that you are installing your new Mukurtu 4 site on the same server as your current Mukurtu 3 site. If you are installing your new Mukurtu 4 site on a different server, please contact us at [support@mukurtu.org](mailto:support@mukurtu.org?subject=Mukurtu%204%20migration%20support)

Go to `/dashboard/migrate` or from the dashboard, select "Migrate from Mukurtu CMS version 3"

![migrate-01](../_embeds/migrate-01.png)

!!! warning
    You will NOT be able to run a migration if there is any content in your new Mukurtu 4 site. A migration can only be attempted on a freshly-built Mukurtu 4 site that has not been used at all.

![migrate-02](../_embeds/migrate-02.png)

Review the preparation steps and select "Continue" when ready.

![migrate-03](../_embeds/migrate-03.png)

Enter the Mukurtu 3 database credentials you identified earlier

- **Database Type**: Likely MySQL or MariaDB.
- **Database Host**: 
- **Database Name**: 
- **Database Username**: 
- **Database Password**: 
- **Document root for public files**: Likely `/var/www/html/your_site/sites/default/files`.
- **Document root for private files**: Likely unused.

Select "Review migration".

![migrate-04](../_embeds/migrate-04.png)

![migrate-05](../_embeds/migrate-05.png)

The migration steps will be displayed. You likely do not need to review these in depth, but the item counts should match your Mukurtu 3 site (eg: number of media assets by type, number of DH items). You may want to take note of these to compare with the migration results.
When ready, select "Begin migration".

![migrate-06](../_embeds/migrate-06.png)

![migrate-07](../_embeds/migrate-07.png)

The migration will run, showing the progress as it goes. 
DO NOT reload, refresh, close, or navigate away from this page until it is complete.

![migrate-08](../_embeds/migrate-08.png)

A confirmation message will be displayed. You may choose to compare the results of the migration to the migration steps earlier.
The content migration is now complete!

![migrate-09](../_embeds/migrate-09.png)
