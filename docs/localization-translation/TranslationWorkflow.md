---
tags:
    - multilingual
    - workflows
---

# Translation Workflow

!!! roles "User roles"
    Mukurtu manager, protocol steward, language steward, contributor, language contributor, curator, community record steward

Mukurtu CMS sites support translation into one or more languages through the Mukurtu Multilingual module. Once the module is configured and a language is added to your site you can translate site components and content in any order you choose, but following this workflow can streamline translation.

Once the Mukurtu Multilingual module is installed and a language is added, site content can be translated. There are several different types of fields that make up content forms in Mukurtu, and they are configured separately. For instance, full HTML fields in content can be translated by inputting the translation directly into the field, but fields that are populated by taxonomy terms must be translated in the taxonomy.

## Configure Mukurtu Multilingual and add languages

Refer to the [Enable Multilingual Mode](ConfigureTranslation.md) article to configure Mukurtu Multilingual and add one or more languages to your site.

## Configure font

Refer to the [Configure Font](ConfigureFont.md) article to configure custom fonts on your Mukurtu CMS site.

## Translate site components

Refer to the [User Interface Translation](UITranslation.md) article for instructions on how to translate your user interface. User interface translation allows a translator to search for specific translated and untranslated strings. Because translation tasks involve many strings, user interface translation allows translators to export, edit, and import translations as a `.po` file.

Refer to the [Configuration Translation](ConfigurationTranslation.md) article for instructions on how to translate all the configuration text on their site that has translatable text, such as the site name, role names, and other structural components.

## Prepare content for translation

### Translate taxonomies

Refer to the [Translate Taxonomies](TranslateTaxonomies.md) article for instructions on how to translate taxonomy vocabularies on your site.

### Translate Local Contexts directory descriptions

Local Contexts project directory descriptions applied Site-wide or to communities or cultural protocols can be translated on Mukurtu no matter which level they are applied. 

!!! tip
    Local Contexts projects and labels must be translated at the Local Contexts Hub. Visit [Local Contexts: Working with the Labels in the Hub](https://localcontexts.org/support/working-with-labels/#customize-labels) for more information.

From your **Dashboard**, navigate to **Manage Local Contexts Projects**. Refer to the [Local Contexts: Using Labels and Notices](../local-contexts/ApplyLabelsAndNoticesToSiteContent.md) to apply your Local Contexts projects. Refer to [Manage Local Contexts Projects](../local-contexts/ManageLocalContextsProjects.md) for how to manage your project directory description. 

Once your Local Contexts projects are applied, navigate to the **Translate project directory settings** tab. 

![Screenshot of the Manage Local Contexts page with the Translate project directory settings tab highlighted.](../_embeds/translatelc1.png)

Enter your translated *Description* text, then select "Save translation". 

![Screenshot of the Translate project directory description modal with the Save translation button highlighted.](../_embeds/translatelc2.png)

## Translate content

!!! tip
    Translating site content can be labor intensive. Best practice is to enable translation for all content when you initially upload it as part of your workflow. You can then go back and translate specific fields. 

For instructions on how to translate content, refer to [Translate Content](TranslateContent.md)

To switch between languages in Mukurtu, you can use the language switcher button in the top right-hand corner of your top menu. The language switcher is only enabled when you have more than one language available on your site.

![Screenshot of the top menu with the language switcher button highlighted.](../_embeds/translation9.png)