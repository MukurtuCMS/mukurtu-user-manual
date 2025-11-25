---
tags:
    - multilingual
---

# User Interface Translation

!!! roles "User role"
    Mukurtu manager

Mukurtu 4 CMS allows users to translate all of their site components into any language and all UTF-8 encoded scripts. Some site components are partially translated by Drupal, but custom fields are not. To translate site components and the user interface in your Mukurtu site, you must have translation configured and have added at least one language. For instructions on how to configure translation, refer to [Configure Translation](ConfigureTranslation.md). For instructions on adding a language to your site, refer to [Add Languages](AddLanguage.md).

User interface translation allows a translator to search for specific translated and untranslated strings, and is used when creating or editing translations. Because translation tasks involve many strings, user interface allows translators to export strings as a .po file for offline editing in a desktop Gettext translation editor, then import the translated strings.

To translate the Mukurtu user interface, navigate to Configuration > Region and Language > User interface translation, or go directly to `/admin/config/regional/translate`.

## Edit translatable strings

You can edit strings individually  on the User interface translation page. 

1. Filter translatable strings by entering part of the string in the *String contains* field. You can leave this field blank to show all strings. 

    !!! tips
        The search is case sensitive. 
    
2. Select your *Translation language* from the dropdown menu.
3. Use the *Search in* field to filter by only translated strings, only untranslated strings, or both translated and untranslated strings.

![Screenshot of the Filter translatable strings fields.](../_embeds/uitranslate1.png)

## Batch edit translatable strings

To streamline your translation workflow, you can batch edit translatable strings by exporting them as a .po file for offline editing in a desktop Gettext translation editor, then import the translated strings. Some examples of Gettext translation editors include:

   - [Poedit.net](https://poedit.net/)
   - [Loco](https://localise.biz/free/poeditor)

Start batch editing your translatable strings by following the instructions below.

1. Select the "Export" button.

    ![Screenshot of the Translation page with Export highlighted.](../_embeds/uitranslate2.png)

2. Select your language and export options from the dropdown menus. You can export non-customized translations, customized translations, untranslated text, or any combination.

    ![Screenshot of the interface translation export page with the Language and Export options fields highlighted.](../_embeds/uitranslate3.png)

3. Select the "Export" button in the top right-hand corner.
4. Open your .po file in your Gettext editor. Make any desired changes, then save your file where you can find it easily.
5. Navigate to your User interface translation page and select the "Import" button.

    ![Screenshot of the User interface translation page with the Import button highlighted.](../_embeds/uitranslate4.png)

6. In the *Translation file* field, select the "Choose File" or "Browse" button to upload your translation file.

    !!! tip
	    Depending on your browser, the text of the button may vary.

7. Select the language you have translated your user interface components into.
8. Select the slider beside each option to determine whether to Treat imported strings as custom translation, Overwrite non-customized translations, or Overwrite existing translations. This can determine whether translations that already exist on the site will be deleted and how imported strings will be treated.

    ![Screenshot of the interface translation import page with the translation file, language, and slider fields highlighted.](../_embeds/uitranslate5.png)

9. Select the Import button to import your user interface translations.