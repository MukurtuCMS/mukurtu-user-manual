---
tags:
    - site settings
---

# Visitor Analytics 

!!! roles "User roles"
    Administrator, Mukurtu manager

Mukurtu has a built-in analytics module that allows administrators to have full control over their site's analytics data.

## Configure Visitor Analytics 

To enable or disable tracking of visitors using the Mukurtu Visitors module, navigate to your **Dashboard** in the **Site settings** section and select the **Analytics settings** link. 

![Screenshot of the Dashboard with the analytics settings link highlighted.](../_embeds/setup4.png)

Tracking is enabled by default. To disable tracking, select the **Disabled** radio button, then select "Save configuration". 

![Screenshot of the visitors configuration page.](../_embeds/setup5.png)

You can also use the Visitors Configuration page to configure:

- Pages - page exceptions
- Roles - user role tracking for specific roles
- Users - turn on or off user opt-out customization
- Entity Counter - which entity types should be tracked
- Retention - how often retention logs are discarded
- Miscellaneous - script type (minified versus full)

### Enable GeoIP 

Optionally, users with command line access can enable the Visitor Analytics module's GeoIP function to show city or regional data. Enabling GeoIP requires a free MaxMind GeoLite2 license key. 

1. Get a MaxMind GeoLite2 license key by creating an account at [maxmind.com](https://www.maxmind.com/en/geolite-free-ip-geolocation-data).
2. Navigate to the GeoIP tab of the **Analytics settings** by selecting the tab or by navigating direcly to `admin/config/system/visitors/geoip`. 
3. Enter your key in the *MaxMind License Key* field.
4. Select "Save configuration".

    ![Screenshot of the Visitors analytics settings page with the GeoIP tab selected and the GeoIP field and Save configuration buttons highlighted.](../_embeds/visitors2.png)

5. Open your terminal and run `drush visitors:download:city`.
6. Then run `drush visitors:rebuild:location` to backfill existing analytics records.
7. In your Mukurtu site, clear your cache by selecting the "Rebuild Cache" button in the top right of your screen.

## View Visitor Analytics

To view analytics provided by the Mukurtu Visitors module, navigate to your **Dashboard** in the **Site settings** section and select the **Analytics** link. 

![Screenshot of the dashboard with the analytics link highlighted.](../_embeds/setup6.png)


