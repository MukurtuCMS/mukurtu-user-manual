---
tags:
    - infrastructure
---

# System Requirements

For the most up-to-date system requirements, please refer to the Drupal 11 [Drupal system requirements](https://www.drupal.org/docs/getting-started/system-requirements/overview#s-drupal-11-and-drupal-cms). We strongly recommend experience installing and maintaining Drupal servers.

Full documentation is also available at [https://github.com/MukurtuCMS/Mukurtu-CMS](https://github.com/MukurtuCMS/Mukurtu-CMS). 

## You will need:

A web server that supports PHP such as Apache or Nginx.

If using Apache make sure that: 

- The `mod_rewrite` module is enabled.
- You have the ability to use local `.htaccess` files. 
- `PHP-FPM` OR `mod_php` must be installed.

If using Nginx make sure that:

- `PHP-FPM` must be installed.
- Create nginx config for Drupal and PHP.

PHP 8.4 or later is required.

A database server using `utf8mb4 / utf8mb4_general_ci` such as:

- [MySQL](https://www.mysql.com/) 8.0 or later.
- [MariaDB](https://mariadb.org/) 10.6 or later.

Private files correctly configured outside the webroot and referenced in `web/sites/default/settings.php`.

A system cron run that runs `drush cron`.

Media tools (recommended). `poppler-utils` (`pdftotext` and `pdftoppm`) for PDF text search and thumbnails, `ffmpeg` for video thumbnails, and PHP's `exec()` must not be disabled. When they're missing, Mukurtu shows a warning on the Status report rather than failing.
