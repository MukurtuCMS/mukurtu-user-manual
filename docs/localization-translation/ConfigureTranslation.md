---
tags:
    - translation and localization
---

# Configure Translation and Localization

!!! roles "User role"
    Mukurtu manager

The following modules should already be included in a standard Mukurtu 4 build, and can be installed from the front end of the site.

- Configuration Translation
- Content Translation
- Interface Translation
- Language Module

## Enable required modules

1. Select **Extend** from the left-hand sidebar menu, or navigate to `/admin/modules`.

    ![Screenshot of the front page with the Extend menu highlighted.](../_embeds/translation1.png)

2. Use the *Filter* field to search for "translation". Three translation modules, Configuration Translation, Content Translation, and Interface Translation, are grouped in the multilingual package.
3. Select all three modules, then select "Install".

    !!! tip
        The Language module should already be installed. If in doubt, search for and install it in the same way.

    ![Screenshot of the Extend menu, with the filter field, checkboxes, and install button highlighted.](../_embeds/translation2.png)

4. You will receive a status message confirming whether your modules have been installed. You will also receive a warning message with the next steps for configuring your Mukurtu site's language.

    ![Screenshot of the Extend menu with the status and warning messages displayed.](../_embeds/translation3.png)

## Add a language

You can add pre-configured or custom languages to your Mukurtu site by following the link in the warning message or by navigating to Configuration > Region and Languages > Language in your left-hand sidebar. You can access this setting directly by going to `/admin/config/regional/language`.

![Screenshot of the Configuration menu with Region and Languages open and Language highlighted](../_embeds/translation7.png)

### Add a pre-configured language

1. Select the "Add Language" button in the top right-hand corner of the Languages configuration page.

    ![Screenshot of the languages configuration page with the add language button highlighted](../_embeds/translation4.png)

2. Select a language to be supported by your site from the dropdown menu. If your language is not listed in the dropdown menu, refer to [Add a custom language code](#add-a-custom-language-code) section of this article for instructions on how to add your language.

    ![Screenshot of the Add language page with the dropdown menu set to French.](../_embeds/translation5.png)

3. Select the "Add language" button to add the selected language to your site.
4. You will receive a confirmation message your language has been added successfully.

    ![Screenshot of the status message confirming that a language has been added successfully.](../_embeds/translation6.png)

### Add a custom language code

1. If your language is not available, select the "Custom language" option to provide a language code and other details manually.

    !!! tip
        More information about constructing custom languages and custom language codes can be found at the [IANA Language Tags Registry](https://www.w3.org/International/articles/language-tags/) site. For more information on constructing custom language tags, visit the [IANA Language Tags Registry https://r12a.github.io/app-subtags/

    ![Screenshot of the Add language page with the dropdown menu set to Custom language...and the fields available](../_embeds/translation8.png)