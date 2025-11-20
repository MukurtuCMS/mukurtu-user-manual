---
tags:
    - translation and localization
---

# Translate Content

!!! roles "User roles"
    Mukurtu manager, protocol steward, language steward, contributor, language contributor, curator, community record steward

Mukurtu 4 CMS allows users to translate all of their site components and content into any language and all UTF-8 encoded scripts. Some site components are partially translated by Drupal, but custom fields and site content are not. To translate components and content in your Mukurtu site, you must have translation configured and have added at least one language. For instructions on how to configure translation, refer to [Configure Translation](ConfigureTranslation.md). For instructions on adding a language to your site, refer to [Add Languages](AddLanguage.md).

## Translate Content

Users can translate all of the content on their site. Follow the instructions below to translate your content.

1. Navigate to the content you want to translate and select the "Translate" button.

![Screenshot of a digital heritage item with the Translate button highlighted.](../_embeds/translatecontent1.png)

2. Select the "Add" button to the right of the language you want to translate your content into. 



## Configuration Translation

Mukurtu managers can translate all the configuration items on their site that has translatable text, such as the site name, role names, and other structural site components. To begin translating these, navigate to Configuration > Region and Language > Configuration Translation, or go directly to `/admin/config/regional/config-translation`.

1. Select the "List" button to the right of the component type you want to translate.

    ![Screenshot of the Configuration Translation page, with List highlighted on the Block component.](../_embeds/translationconfig1.png)

2. Select the "Translate" button to the right of the specific site component you want to translate. Use the *Search* field to search for specific site components. 

    ![Screenshot fo the Block page, with the Search field and the Translate button to the right of Page Title highlighted](../_embeds/translationconfig2.png)

3. If your site component is not translated, select the "Add" button to add a translation. If it is already translated, select the "Edit" button to edit the translation.

    ![Screenshot of the Translation page with English, French, and Gaeilge](../_embeds/translationconfig3.png)
    
4. Enter your preferred translation, then select "Save translation".

    ![Screenshot of the Edit Translation modal with the translation entered in French.](../_embeds/translationconfig4.png)

## User Interface Translation

User interface translation allows a translator to search for specific translated and untranslated strings, and is used when creating or editing translations. Because translation tasks involve many strings, user interface allows translators to export strings for offline editing in a desktop Gettext translation editor, then import the translated strings.



