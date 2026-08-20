---
tags: 
    - migration
---

# 5) Stage and import Mukurtu 3 files and database

## Configure database settings

In your Mukurtu 4 install access `/web/sites/default/settings.php`, find the section "Database settings" and replace what's there with the following. Note that name_of_v3_site must match the directory name of the Mukurtu 3 site you downloaded earlier.

    $databases = [];
    $host = "db";
    $port = 3306;
    $driver = "mysql";
    $databases['migrate']['default'] = [
        'database' => 'name_of_v3_site',
        'username' => 'root',
        'password' => 'root',
        'host' => $host,
        'port' => $port,
        'driver' => $driver,
        'prefix' => '',
        'collation' => 'utf8mb4_general_ci',
    ];

## Place Mukurtu 3 directory and database into Mukurtu 4 environment

Place the Mukurtu 3 directory you prepared earlier within the `web` directory of your Mukurtu 4 project. This must match the `name_of_v3_site` provided in the database settings.

- The path will be something like `mukurtu4/web/name_of_v3_site`

Locate the Mukurtu 3 database you prepared earlier. You can place it in the Mukurtu 4 project root for ease of reference, or just make note of it's path. Extract the .sql.gz file so that the .sql file is accessible. It will be something like `my_v3_db.sql`

- The path will be something like `mukurtu4/my_v3_db.sql`

## Import Mukurtu 3 database

In a terminal open to the root of the Mukurtu 4 project, run: `[project] import-db --database=<v3 site name> --file=<db name.sql>`

- If you placed the database file in your Mukurtu 4 project root, it would look something like: `mukurt4 import-db --database=name_of_v3_site --file=my_v3_db.sql`

Notes:

- Don't forget the `--database=name_of_v3_site` part! It should match what you entered in the database settings above. If you don't specify this, the command will overwrite the default "db" database, which is bad since that's your v4 database! If you wipe that, you won't be able to run a migration. We need a v3 and a v4 database side by side in order for it to work.
- .sql is only one possible format you can have for the dump file. Run `[project] import-db --help` to get a full list of accepted formats.