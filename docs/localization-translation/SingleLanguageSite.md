---
tags:
    - multilingual
---

# Configure a Non-English Mukurtu Site

!!! roles "User role"
    Mukurtu manager

Mukurtu CMS sites can be configured to display in any language. To configure your site to only display in your language, follow the instructions below.

1. [Configure Translation](ConfigureTranslation.md/#configure-translation) for your site and [add a language](ConfigureTranslation.md/#add-a-language).
2. After adding your language, set it to default by selecting the radio selector to the right of your language in the Default column. 

    ![Screenshot of the language selection screen with the radio selector highlighted.](../_embeds/nonenglish1.png)

3. Select "Save Configuration". 
4. Disable or remove the language switcher block by navigating to your administrative menu and select Structure > Block layout or navigating directly to `/admin/structure/block`. 
5. Under the User menu in the *Language switcher (Content)* field, use the dropdown menu to select Disable or Remove. 

    ![Screenshot of the dropdown menu with Disable selected.](../_embeds/nonenglish2.png)

You will get a status message confirming that the block settings have been updated.

   ![Screenshot of the confirmation status message](../_embeds/nonenglish3.png)

5. The language switcher can also be removed by selecting the edit option to the left of the language switcher block. Select the **Edit** icon, then select the **Remove block** option.

    ![Screenshot of the front page with the edit icon by the language switcher block highlighted](../_embeds/noenglish4.png)

    ![Screenshot of the edit dropdown with the Remove block option selected.](../_embeds/noenglish5.png)

6. Refer to the [Configuration Translation](ConfigurationTranslation.md) and [User Interface Translation](UITranslation.md) articles to translate any configuration or user interface strings.
7. New content does not need to be translated, and can simply be added in your preferred language.

