---
tags:
    - site maintenance
---

# Check for Drupal Database and Module Updates

!!! Roles "User roles" 
    Administrator

This article provies instructions for checking for updates within a Mukurtu site and configuring update notifications. For instructions on updating a site, see [Update a Reclaim Hosted Site](../site-maintenance/UpdateAReclaimHostedSite.md) and [Update a Self-Hosted Site](../site-maintenance/UpdateASelfHostedSite.md) 

To check for Drupal database updates and module updates, go to `admin/reports/updates` 

You can also access the udpates page by hovering over the reports menu and selecting "Available Updates"

![The reports menu with Available Updates highlighted](../_embeds/check-for-updates-01.png)

## List

The available updates page has two tabs. In the list tab, you will see available updates for Drupal Core, followed by a list of installed modules and themes. You can also check for updates manually by selecting the **Check Manually** link. Items in green are up to date. Items in yellow have updates available. Some modules may require a Drupal update before they can be updated.

![The available updates page showing updates for drupal core. Above drupal core is a check manually link that can be used to check for updates ](../_embeds/check-for-updates-02.png)

![The available udpates pages showing the list of installed modules and themes](../_embeds/check-for-updates-03.png)

## Settings

The settings tab has several settings you can configure. You can:

- Select whether you want to check for updates daily or weekly. By default the system will check daily.

- Decide to check for updates on uninstalled modules or themes.

- Add an email address that will be notified when updates are available.

- Decide what you want to receive notifications for: all newer versions or security updates only.

![The settings tab. Listed are several configurations: Select daily or weekly updates, check for updates on uninstalled modules or themes, add an enamil address for notification, and receive notifications for new versions or security updates only. ](../_embeds/check-for-updates-04.png)

When you've made your selections, select "Save configuration." The page will reload with a success message.