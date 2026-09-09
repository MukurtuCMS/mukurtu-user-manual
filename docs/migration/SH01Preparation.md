---
tags: 
    - migration
---

# Prepare migration information

!!! warning
    This documentation assumes that you are installing your new Mukurtu 4 site on the same server as your current Mukurtu 3 site. If you are installing your new Mukurtu 4 site on a different server, please contact us at [support@mukurtu.org](mailto:support@mukurtu.org?subject=Mukurtu%204%20migration%20support)

## Documenting customization

If you have undertaken any customization of Mukurtu we strongly encourage you to document all your changes, whether cosmetic or functional. You will want to have a clear list of modifications so that you can identify what needs to be migrated, what needs to be re-created, etc.

Please contact us at support@mukurtu.org so that we can discuss your options and needs for migration and re-implementation. There will not be a one-size-fits-all solution, but we plan to document the common customizations reported by users and make workflows, tools, and any other resources available to all users to support everyone's migration efforts.

Customization includes, but may not be limited to:

- Adding new fields to existing content types.
- Disabling fields on existing content types.
- Modifying the data structure of existing fields.
- Creating new content types.
- Installing additional modules.
- Modifying any stock configuration (eg: user role permissions, search API).
- Modifying certain look and feel modifications (eg: navigation menu, content view modes).

!!! warning
    Custom themes and other look and feel modifications wil NOT be migrated. Custom themes will need to be re-designed and re-implemented to use the Drupal 11 Twig theming environment. This is beyond our capacity to support.

## Locating needed information

You will need to collect file locations and database credentials from your Mukurtu 3 site for use in your eventual migration. We recommend reviewing this well in advance and recoding this information somewhere accessible so you can copy and paste it into your new Mukurtu 4 site when prompted.

You will need the following information:

- Location of your Mukurtu 3 installation
    - Document root for public files
    - Document root for private files
- Database information 
    - Database type
    - Database host
    - Database name
    - Database username
    - Database password

### Location of your Mukurtu 3 installation

The location of your Mukurtu 3 install is dependant on how your system administrator configured the web server. A common location is `/var/www/html/your_site`, but you will want to verify this.

Once you have the the location of your site you can find most of the rest of the information you need.  

**Document root for public files**
The location of your public files will be in `/var/www/html/your_site/sites/default/files` 

**Document root for private files**
To find the Private file system path (this is not always used) login to your site. Then navigate to https://your.site/admin/config/media/file-system. Look for the text box labeled "Private file system path". If it is empty you are not using Private files. If it is filled in note the location that is listed.

### Database information

To find your database information you will need to use the command line. Then change to the "default" directory of your site. Using the example provided above you would:

    cd /var/www/html/your_site/sites/default/
    cat settings.php

Look for the section that looks similar to this:

    $databases = array (
        'default' =>
        array (
            'default' =>
                array (
                    'database' => 'database_name',
                    'username' => 'database_user',
                    'password' => 'password',
                    'host' => 'server',
                    'driver' => 'mysql',
                    'prefix' => '',
                ),
        ),
    );

Take note of the following:

    'database' => 'database_name',
    'username' => 'database_user',
    'password' => 'password',
    'host' => 'server',


