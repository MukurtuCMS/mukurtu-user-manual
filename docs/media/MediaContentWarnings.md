---
tags: 
    - media
---
# Media Content Warnings

!!! roles "User role"
    Mukurtu administrator

Media content warnings are a specific type of media tag that enables Mukurtu administrators to flag potentially sensitive media assets. There are two different types of media content warnings: taxonomy triggered warnings and deceased person warnings. When a user comes to a page with a media asset that has a content warning, they are presented with a blacked-out box in place of the media asset overlaid with descriptive text. The user can choose to click through to access the media. This feature does not prevent users from accessing media assets, but it presents them the choice to access it if they want to after being made aware of its sensitive nature. 

Media content warnings can be applied in many different ways according to the community's needs. Some communities may decide to apply person warnings to let community members know that they may be viewing media that has images or recordings of persons who are deceased. Some ways that communities have chosen to apply taxonomy triggered media content warnings are as trigger warnings to inform users of media assets that might have violent or triggering content for some users. 

Creating media content warnings is a multi-step process. These parts need to be done in the order they are presented here to generate media content warnings and apply them to your media assets. 

Sites can have many different media content warnings configured, and media assets can have more than one media content warning applied. 

A completed media content warning can look like this:

![Screenshot of a media content warning applied to a media asset in a digital heritage item](../_embeds/placeholderscreenshot.png)

To begin, navigate to your dashboard. 

## Taxonomy triggered warnings

### Create a media tag

1. Under the **Additional content settings** section of the dashboard, select the **Manage Taxonomies** link or go directly to `/admin/structure/taxonomy`

    ![Screenshot of where the manage taxonomies link is located in the dashboard](../_embeds/placeholderscreenshot.png)

2. Navigate to the **Media Tag** link. Your media tag will act as the term, or name, for your content warning, so choose a tag that clearly communicates the type of warning you want to apply.
3. Select the "Add a new term in Media Tag" button.
4. Use the *Name* field to enter a name for your media content warning.
5. Use the *Description* field to enter a description of the media tag for your media content warning. The description could help distuinguish between media tags or describe the type of media assets they should be applied to.

    ![Screenshot of the name and description fields with sample text filled in](../_embeds/placeholderscreenshot.png)

6. Select the "Save" button to save your media tag.
7. Navigate back to your dashboard to complete creating your media content warning.

### Create a content warning

1. Under the **Media** section of the dashboard, select the **Content Warnings Settings** link or go directly to `/admin/config/mukurtu/content-warnings`

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

2. Navigate to the **Taxonomy Triggered Warnings** section. 
3. Select the "Add taxonomy warning" button. 

    ![Screenshot of where the taxonomy triggered warnings link is located in the content warnings settings ](../_embeds/placeholderscreenshot.png)

4. Select a **Term** from the dropdown menu. Terms are media tags attached to the media that will trigger the warning. They are configured in under **Taxonomy** as media tags, and are the required name of your media content warning. 

    !!! requirement
        If you have not created a term for your media content warning, navigate to the **Generate a media tag** section of this article for instructions.

5. Once you have selected your term, apply warning text. In the *Warning Text* field enter the warning text you would like displayed on your media overlay. This field has a 255 character limit.

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

6. Select the "Submit" button to save your media content warning.

## Deceased person warnings

There are several steps to create a deceased person warning, including enabling the person taxonomy, creating a person record, and creating a taxonomic people term. For further information about how to create person records, visit [Create a Person Record](PersonRecords.md). For further instructions on how to create deceased person media content warnings, follow the instructions below.

### Create a people term

1. Navigate to **Mukurtu Taxonomy Record Settings** from your dashboard or go directly to `/admin/config/mukurtu/taxonomy/records` to enable the person taxonomy. Select the checkbox beside the *Person* field to make sure this taxonomy is enabled, then select the "Save configuration" button.
2. Navigate to your dashboard. Under the **Additional content settings** section of the dashboard, select the **Manage Taxonomies** link or go directly to `/admin/structure/taxonomy`

    ![Screenshot of where the manage taxonomies link is located in the dashboard](../_embeds/placeholderscreenshot.png)

3. Navigate to the **People** link. Your people taxonomy term acts as the trigger for the person warning.
4. Select the "List terms" button.
5. Select the "Add term" button. 
6. Use the *Name* field to enter the name of the person.
7. Use the *Description* field to enter a description of the person. The description could help distuinguish between people who have similar names or record other notes.

    ![Screenshot of the name and description fields with sample text filled in](../_embeds/placeholderscreenshot.png)

8. Select the "Save" button to save your people tag.
9. Navigate back to your dashboard to complete creating your media content warning.

### Create a person record

To apply a person warning to a media asset, the *deceased* box must be checked and the person's name must be entered as a taxonomic term in the **representative terms** section. 

1. Create a person record according to the instructions here **MAKE A CREATE A PERSON RECORD LINK AND INSERT IT HERE**.
2. Make sure the *Deceased* box is selected. In the **Mukurtu Essentials** tab, mark the checkbox by *Deceased*.
3. Make sure the person's name has been entered in the **Representative Terms** section as a taxonomic term. 

    - Navigate to the **Relations** tab.
    - In the **Representative Terms** section, select the "Select Terms" button. Enter your search term or select the term from the list below by selecting the checkbox by the person's name.
    - Select the "Add Terms" button to add the person's name as the representative term in the person record. More than one taxonomic term can be applied.

    !!! requirement
        If you have not enabled the person taxonomy, this field will not populate. Navigate to the **Create a people term** section of this article for instructions.

        If you have not created a taxonomic people term, navigate to the **Create a people term** section of this article for instructions.

    ![Screenshot showing the add terms pop-up with a person's name selected](../_embeds/placeholderscreenshot.png)

5. Select the "Save" button to save your person record. 

### Create a person warning

1. Under the **Media** section of the dashboard, select the **Content Warnings Settings** link or go directly to `/admin/config/mukurtu/content-warnings`

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

2. Navigate to the **People Warnings** section and select the checkbox beside **Enable People Warnings**. 
3. In the *Warning Text: Single Person* field, enter the text to be displayed on the media overlay for a single deceased person. Use the replacement token `[name]` to automatically insert the person's name in the text. An example of warning text for a single person is `Warning: [name] is deceased. Click through to access content.`
4. In the *Warning Text: Multiple People* field, enter the text to be displayed on the media overlay for a media asset displaying multiple deceased individuals. Use the replacement token `[names]` to automatically insert the people's names in the text. An example of warning text for multiple people is `Warning: The following people are deceased. Click through to access content. [names]`

![Screenshot showing how to fill out the enable people warnings and warning text fields.](../_embeds/placeholderscreenshot.png)

## Apply a media content warning

!!! roles "User roles"
    Protocol steward, contributor, community record steward, curator, language steward, language contributor 

Follow these steps to apply a media content warning to a media asset.

1. Navigate to the media asset you want to apply the media content warning to through your dashboard or through editing the media asset from a content item. You can also apply a media content warning when you create a new media asset. For instructions on how to create a new media asset, visit the [Media Upload Instructions by Media Type](ByTypeMediaUpload.md) article.

    - From your dashboard, navigate to the **Media** section and select the **Manage Media** link. 
        - Under the **Operations** heading, select the "Edit" button from the dropdown button menu.
    - From a content item, select a content item. 
        - Select the small, round edit button on the top right of the media asset. When you select it, it will present a dropdown menu with the options edit or delete the media asset. Select the **Edit** link.

        ![Screenshot of a media asset showing the location of the edit button](../_embeds/placeholderscreenshot.png)

    - From a new media asset, follow the steps outlined in the [Media Upload Instructions by Media Type](ByTypeMediaUpload.md) article to apply media tags.

2. To enter a taxonomy triggered media content warning, navigate to the **Media Tags** section of your media asset. Begin entering the term for your media content warning. Your selection should display in the dropdown. 
3. To enter a deceased person content warning, navigate to the *People* field in your media asset. Begin entering the name of the person. Your selection should display in the dropdown. 
4. If more than one media content warning media tag, or person's name needs to be applied to the media asset, select the "Add another item" button.
5. Select the "Save" button to save your media asset with a newly applied media content warning.

![Screenshot of a digital heritage item with a taxonomy triggered media content warning applied](../_embeds/placeholderscreenshot.png)

![Screenshot of a digital heritage item with a person warning media content warning applied](../_embeds/placeholderscreenshot.png)