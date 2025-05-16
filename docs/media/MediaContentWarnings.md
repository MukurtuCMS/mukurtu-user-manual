---
tags: 
    - media
---
# Media Content Warnings

!!! roles "User role"
    Mukurtu administrator

Media content warnings are a tool used to flag potentially sensitive or triggering media assets, and allow a user to choose whether or not to interact with them before viewing or accessing the media. They can be used with all media types, and configured to display with thumbnails, full-size media, and other display modes.

When a user is presented with a media asset that has a content warning, it will be replaced with a blacked-out box and descriptive warning text. At that point, the user can choose to dismiss the warning and access the media, or leave the warning in place. This feature does not replace or bypass cultural protocols on media assets, rather it presents them the choice to access it if they want to after being made aware of its sensitive nature. This also does not affect the rest of the page contents, so if a digital heritage item includes a media asset with a content warning, that does not extend to the metadata or other media assets in that item.

There are two types of media content warnings: taxonomy triggered warnings and deceased person warnings. Both can be active on one site, and they are configured separately.

Taxonomy triggered warnings
Taxonomy triggered warnings are the more flexible of the two types of warnings. They are dependent on the *media tags* field that is included in all media types. You can configure as many different taxonomy warnings as necessary. Each warning is composed of the trigger media tag, and a customized message.

Some example uses of taxonomy triggered warnings include boarding or residential school materials, graphic or violent text or images, offensive or racist language and representation, or materials that may otherwise make users uncomfortable.

Deceased person warnings
Deceased person warnings are a more rigid warning. They are dependent on the people field that is included in all media types, and require use of the person record [add link] tool. There is only one deceased person warning available, and the message can be customized.

!!! tip
     Deceased person warnings are a response to requests from communities where there are degrees of restrictions on how individuals can or should interact with images or recordings of people who have passed away. If the choice is individual this is a useful tool, however if there is need for stricter control over access to these materials, consider managing that with cultural protocols.

Creating media content warnings is a multi-step process. These parts need to be done in the order they are presented here to generate media content warnings and apply them to your media assets. 

Sites can have many different media content warnings configured, and media assets can have more than one media content warning applied. 

A completed media content warning can look like this:

![Screenshot of a taxonomy triggered media content warning applied to a media asset in a digital heritage item](../_embeds/placeholderscreenshot.png)

![Screenshot of a deceased person media content warning applied to a media asset in a digital heritage item](../_embeds/placeholderscreenshot.png)

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

### Configure a taxonomy warning

1. Under the **Media** section of the dashboard, select the **Content Warnings Settings** link or go directly to `/admin/config/mukurtu/content-warnings`

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

2. Navigate to the **Taxonomy Triggered Warnings** section. 
3. Select a **Term** from the dropdown menu. Terms are media tags attached to the media that will trigger the warning. They function as the name of your media content warning. 

    ![Screenshot of where the taxonomy triggered warnings link is located in the content warnings settings ](../_embeds/placeholderscreenshot.png)

4. Select the "Add taxonomy warning" button to add additional taxonomy warnings. 
5. Once you have selected your term, apply warning text. In the *Warning Text* field enter the warning text you would like displayed on your media overlay. This field has a 255 character limit.

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

6. Select the "Submit" button to save your media content warning.

To apply a taxonomy based media content warning, navigate to the [Apply a media content warning](#apply-a-media-content-warning) section of this article.

## Deceased person warnings

There are several required steps to create a deceased person warning, including:

- enabling the person taxonomy
- creating a taxonomic people term
- creating a person record

For further information about how to create person records, visit [Create a Person Record](../person-records/PersonRecords). For further instructions on how to create deceased person media content warnings, follow the instructions below.


### Configure person warnings

1. Under the **Media** section of the dashboard, select the **Content Warnings Settings** link or go directly to `/admin/config/mukurtu/content-warnings`

    ![Screenshot of where the content warnings settings link is located in the dashboard](../_embeds/placeholderscreenshot.png)

2. Navigate to the **People Warnings** section and select the checkbox beside **Enable People Warnings**. 
3. In the *Warning Text: Single Person* field, enter the text to be displayed on the media overlay for a single deceased person. Use the replacement token `[name]` to automatically insert the person's name in the text. An example of warning text for a single person is `Warning: [name] is deceased. Click through to access content.`
4. In the *Warning Text: Multiple People* field, enter the text to be displayed on the media overlay for a media asset displaying multiple deceased individuals. Use the replacement token `[names]` to automatically insert the people's names in the text. An example of warning text for multiple people is `Warning: The following people are deceased. Click through to access content. [names]`

![Screenshot showing how to fill out the enable people warnings and warning text fields.](../_embeds/placeholderscreenshot.png)

5. Navigate to the bottom of the page and select the "Submit" button to save your media content warnings.

### Configure person record settings

1. For instructions on how to enable the person taxonomy, visit [Configure Person Record Settings](../person-records/ConfigurePersonRecord.md). The person taxonomy must be enabled before you can create people terms.
2. Once the taxonomy is enabled, people terms can be drawn from content and media as they are created. If you have not created people terms directly from content and media, follow the instructions below to add people terms directly to your taxonomy.
3. Navigate to your dashboard. Under the **Additional content settings** section of the dashboard, select the **Manage Taxonomies** link or go directly to `/admin/structure/taxonomy`

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

Create a person record according to the instructions here [Create a Person Record](../person-records/PersonRecords). To apply a person warning to a media asset, the *deceased* box must be checked and the person's name must be entered as a taxonomic term in the **representative terms** section. Follow the instructions to make sure your person record is configured to apply a deceased person warning.

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