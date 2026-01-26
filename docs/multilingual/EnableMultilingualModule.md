---
tags:
    - multilingual
---

# Enable Multilingual Module

!!! roles "User role"
    Mukurtu manager

The Mukurtu Multilingual module enables the required Drupal multilingual modules (Configuration Translation `/admin/config/regional/config-translation`, Interface Translation `/admin/config/regional/translate`, and Content Translation`/admin/config/regional/content-language`), and configures recommended default settings for most multilingual work. If necessary, these settings can be modified after enabling the Mukurtu Multilingual module.Follow the instructions below to configure your site to display your site's elements and content in multiple languages. 

## Enable module

1. From the administrative menu, select **Extend** or navigate to `/admin/modules`.

    ![Screenshot of the front page with the Extend menu highlighted.](../_embeds/translation1.png)

2. Use the *Filter* field to search for "multilingual". 
3. Select Mukurtu Multilingual, then select "Install". This installs and configures the Mukurtu Multilingual, Configuration Translation, Interface Translation, and Content Translation modules.

    ![Screenshot of the Extend menu, with the checkbox and install button highlighted.](../_embeds/translation2.png)

4. You will receive a message asking you to confirm that you want to install all of the associated modules. Select "Continue".

    ![Screenshot of the message asking you to confirm whether you want to install all of the multilingual modules.](../_embeds/translation3.png)

5. You will receive a status message confirming whether your modules have been installed. The warning message includes a link to add languages to your Mukurtu site. For instructions on adding languages to your Mukurtu site, refer to [Add Languages](#AddLanguage).

    ![Screenshot of the Extend menu with the status and warning messages displayed.](../_embeds/translation3a.png)

## Add Languages

To add another language for translation, follow the link in the warning message you got when you configured your site languages or use the administrative menu to navigate to Configuration > Region and Languages > Language. You can also access this setting directly by going to `/admin/config/regional/language`. For more information on configuring translation, refer to [Configure Translation](ConfigureTranslation.md)

![Screenshot of the Configuration menu with Region and Languages open and Language highlighted](../_embeds/translation7.png)

### Add a language

1. Select the "Add Language" button in the top right-hand corner of the Languages configuration page.

    ![Screenshot of the languages configuration page with the add language button highlighted](../_embeds/translation4.png)

2. Select a language from the dropdown menu. If your language is not listed in the dropdown menu, refer to [Add a custom language code](#add-a-custom-language-code) section of this article for instructions on how to add your language.

    ![Screenshot of the Add language page with the dropdown menu set to French.](../_embeds/translation5.png)

3. Select the "Add language" button to add the selected language to your site.
4. You will receive a confirmation message your language has been added successfully.

    ![Screenshot of the status message confirming that a language has been added successfully.](../_embeds/translation6.png)

### Add a custom language

1. If your language is not available, select the "Custom language" option to provide a language code and other details manually. For more information on translating site elements, refer to the [Configuration Translation](ConfigurationTranslation) and [User Interface Translation](UITranslation.md) articles.

    - A listing of IANA language tags can be found at the [IANA Language Tags Registry](https://r12a.github.io/app-subtags/) site. 
    - If your language is not listed, you can construct a custom language tag. For more information on constructing custom language tags, visit the [IANA Language Tags Registry](https://www.w3.org/International/articles/language-tags/). 

2. Add your language code in the *Language code* field.
3. Add the name of your language in the *Language name* field. 
4. Select a text direction for your language. 
5. Select the "Add custom language" button to import your language.
        
For more information on language tags and subtags, visit the [IANA Language Tags Registry Primary Language Subtag](https://www.w3.org/International/articles/language-tags/#language) article. For help configuring a custom language tag, please contact Mukurtu Support at [support@mukurtu.org](mailto:support@mukurtu.org).

![Screenshot of the Add language page with the dropdown menu set to Custom language...and the fields available, filled in and highlighted, as well as the text direction and Add language button.](../_embeds/translation8.png)