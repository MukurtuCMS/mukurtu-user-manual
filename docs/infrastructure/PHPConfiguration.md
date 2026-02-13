---
tags:
    - infrsutructure
---

# PHP Configuration 

For most Mukurtu sites to run properly, the PHP memory_limit must be set to a minimum of 196 MB. For larger sites, 256 MB is recommended. The max_execution_time should be set to a minimum of 90 or 120 seconds.

If you are using Reclaim Hosting, follow the directions below to view and change your memory_limit setting. If your site is hosted elsewhere, contact your site administrator and/or hosting provider.

Login to the Reclaim client portal: [https://portal.reclaimhosting.com/clientarea.php](https://portal.reclaimhosting.com/clientarea.php)

![The Reclaim login page showing the username and password fields and login button](../_embeds/php-config-01.png)

Go to the cPanel.

![The Reclaim dashboard. The cPanel menu is located in the main navigation menu](../_embeds/php-config-02.jpg)

Search or browse for the MultiPHP INI editor.

![A page listing several different available tools organized by type. The MultiPHP INI editor is located in the Software section](../_embeds/php-config-03.png)

Select the location of your site. This may be your site URL, or be listed as “Home Directory”.

![Home Directory is selected in the drop-down menu under Configure PHP INI basic settings](../_embeds/php-config-04.png)

Locate the max_execution_time field and set it to 90 (or 120 if needed), and memory_limit field and set it to 196M (or 256M if needed).

![A list of PHP directives. Max_execution_time and memory_limit are both highlighted](../_embeds/php-config-05.png)

Select "Apply" at the bottom of the screen.

It may take a few minutes for the changes to affect your site.

