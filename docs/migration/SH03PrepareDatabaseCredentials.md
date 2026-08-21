---
tags: 
    - migration
---

# 3) Prepare Mukurtu 3 database and credentials

## Documenting customization

If you have undertaken any customization of Mukurtu we strongly encourage you to document all your changes, whether cosmetic or functional. You will want to have a clear list of modifications so that you can identify what needs to be migrated, what needs to be re-created, etc.

Please contact us at [support@mukurtu.org](mailto:support@mukurtu.org) so that we can discuss your options and needs for migration and re-implementation. There will not be a one-size-fits-all solution, but we plan to document the common customizations reported by users and make workflows, tools, and any other resources available to all users to support everyone's migration efforts.

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

## Download the Mukurtu 3 project directory

You will need the complete directory of the Mukurtu 3 site so that the media assets and other components can be migrated into Mukurtu 4.

## Export/dump the Mukurtu 3 database

You need to dump or export the SQL database from your Mukurtu 3 site so that the contents can be migrated into Mukurtu 4.

This is usually done with a command `like export-db -f my_v3_db.sql` from the project root in a terminal.

## Preparing migration credentials

You will need to collect database credentials from your Mukurtu 3 site for use in your eventual migration. We recommend reviewing this well in advance and recoding this information somewhere accessible so you can copy and paste it into your new Mukurtu 4 site when prompted.

You will need to prepare the following database settings and credentials.

- Database type
- Database host
- Database name
- Database username
- Database password
- Document root for public files
- Document root for private files

!!! tip
    This assumes that you are migrating within the same hosting environment. If you are changing hosting providers or hosting environments please contact [support@mukurtu.org](mailto:support@mukurtu.org).

### Finding database credentials

Contact your server/system administrator. They should be directly involved in this process. If they have any questions about this information or the migration process, please contact [support@mukurtu.org](mailto:support@mukurtu.org).

!!! warning
    Use command line tools with caution. If you are not familiar with command line tools contact your server/system administrator or use other tools.

Change to the directory with your Mukurtu settings.php file.

- On most hosts it will be something like /var/www/html/[sitename]/sites/default/files
- On Reclaim it will likely be either
  - For a single domain or sub-folder install (eg: mydomain.com or mydomain.com/mukurtusite): /public_html/[sitename]/sites/default
  - For a subdomain install (eg: mukurtusite.mydomain.com): /public_html/[sitename]/sites/default

For example, ```cd /var/www/html/[sitename]/sites/default/files```, ```cd public_html/[sitename]/sites/default```, or ```cd public_html/[sitename]/sites/default```.

Then run the cat command to display the contents of the settings.php file.

```cat settings.php```

Look for the database information. It will look something like this, and is *usually* the last information displayed.

```
$databases = array (
  'default' =>
  array (
    'default' =>
    array (
      'database' => '[database_name]',
      'username' => '[username],
      'password' => '[secret_password],
      'host' => 'localhost',
      'port' => '',
      'driver' => 'mysql',
      'prefix' => '',
    ),
  ),
);
```

Record this information. We recommend copying this into a local text document for future reference.

