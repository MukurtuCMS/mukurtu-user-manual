---
tags:
    - content
    - person records
    - taxonomy
---
# Create Person Records

!!! roles "User roles"
    Protocol steward, contributor

Person Records allow for rich biographical records to be integrated into Mukurtu CMS. Person records can include birth and death dates as well as custom text and media sections. They can also identify relationships between people, and aggregate all digital heritage items where a person is referenced. They can also be used to link all the names that a person is known to the record as taxonomic people terms. Follow the instructions below to create a person record.

!!! requirement
    If you have not enabled the person taxonomy, this field will not populate. Navigate to the [Configure Person Record Settings](person-records\ConfigurePersonRecord.md) article for instructions. 

From your **Dashboard** or **Add Content**, select the **Person** link.

## Mukurtu Essentials

### Name - required

Enter the preferred name of the person in the *Name* field. Names can be formatted as `Last, First, Middle`, `Last, First (Nickname)`, `Family name, Given name`, or any other format that makes sense for your community.

- This is a required field.

### Media assets

Add featured media to the **Media Assets** section by selecting the "Add media" button. This can be unique or can reuse media from other content. There is no limit on the number of media assets you can add.

1. To upload a media asset, navigate to the Media Assets section.
2. Select the "Add Media" button.
3. Select the type of content you want to add. You can upload an audio file, document, image, or video file.
4. Select the "Choose File" or "Browse" button to upload a file.
        
    !!! Tip
        The text of the upload button depends on your browser.

5. Select an file from your file explorer.
6. If you selected the incorrect file, remove it by selecting the "Remove" button after the file uploads.
7. Fill out the remaining metadata according to the [Media Upload Instructions by Media Type](../media/ByTypeMediaUpload.md) article.

![Screenshot with a media asset applied.](../_embeds/placeholderscreenshot.png)

### Sharing settings - required

1. Navigate to the **Sharing Setting** field to apply a sharing setting. Select **All** or **Any**.

    - All means that the item may only be shared with members belonging to ALL the protocols listed. This is the more restrictive setting. 
    - Any means the asset may be shared with members of ANY of the protocols listed. This is less restrictive.
    - This is a required field.

2. Use the checkboxes to apply cultural protocols to the media asset.

    - This is a required field.

![Screenshot with the sharing setting and cultural protocols selected.](../_embeds/placeholderscreenshot.png)

### Date fields

1.  In the **Date Born** section enter the date the person was born. Acceptable formats are `YYYY`, `YYYY-MM`, or `YYYY-MM-DD`.
2. In the **Date Died** section enter the date the person died. Acceptable formats are `YYYY`, `YYYY-MM`, or `YYYY-MM-DD`.
3. Use the checkbox to indicate whether the person is **Deceased**. This field informs the deceased person media content warning. For more information on this and other media content warnings, please see the [Media Content Warnings](../media/MediaContentWarnings.md) article.

![Screenshot of the date and deceased fields with information filled in to indicate the dates the person was born and died, and that the individual is deceased.](../_embeds/placeholderscreenshot.png)

### Keywords

In the **Keywords** section, add keywords to each field to describe the person. Keywords provide an additional way to categorize your content. In general, 3-5 keywords are recommended to make it easier for users to search and retrieve content. 
   
1. Select the "Add another item" button to add additional keyword text boxes.
2. Select and drag the arrows by the keyword to reorder your keywords if necessary.
3. To remove a keyword, select the "Remove" button.

### Mapping and location

1. Use the **Map Points** Leaflet map to enter one or more geographic locations for your person record. This can be an area that the person lived in, that they were associated with, or any other geographic location. Use the buttons on the right to enter points, paths, rectangles, or polyons to your map. You can also add markers to your map by uploading GeoJSON shapes. For more information on how to use the **Map Points** Leaflet map, visit **INSERT AN ARTICLE ON MAPPING HERE**
2. Add a *Location Description*. If a location has identifying characteristics but is not able to be pinpointed on a map this field can be used instead of the mapped location. It can also be used to add additional context to the map points. This is a full HTML field that also supports additional media.
3. Use the *Location* field to provide a taxonomic location term for your collection.

    - Select the "Add another item" button to add additional location text boxes.
    - Select and drag the arrows by the location to reorder your locations if necessary.
    - To remove a location, select the "Remove" button.

    ![Screenshot of the location description and taxonomic location fields filled in.](../_embeds/placeholderscreenshot.png)

### Local Contexts

Use the *Local Contexts* field to apply Traditional Knowledge labels to your collection. 
    
!!! tip
    To start a project or for more information on Local Contexts projects, labels, and notices, visit [Local Contexts](https://localcontexts.org/).

1. Select your Local Contexts project from the dropdown. 
2. Select Local Contexts labels and notices to assign to the collection.  
      
![Screenshot of the local contexts fields with information selected from the dropdown menu.](../_embeds/placeholderscreenshot.png)

You can save your person record at this point, or return to the top of your page to select the **Text Sections** or **Relations** tabs to add more context to your person record.

## Text Sections

This is where you can provide biographical information for your person record. 

1. Under the **Biographical Information Sections**, enter the title of the biographical information in the *Title* field. 
2. Use the *Body* field to provide a longer biographical sketch for your person record. This field enables a broader narrative that can include a written biography, audio recordings, video recordings, images, or any other supportive information for your person record. This is a full HTML field that supports text, audio, images, and video media assets.
3. Select the "Add Formatted Text with Title" button to add an additional biographical information section. 

    !!! tip
        Adding multiple biographical information sections allows users a more clearly delineated way to provide multiple people's perspectives on the individual's life or separate different aspects of their life, activities, or work.

![Screenshot with the text sections and biographical information sections filled in with example text.](../_embeds/placeholderscreenshot.png)

You can save your person record at this point, or return to the top of your page to select the **Mukurtu Essentials** or **Relations** tabs to add more context to your person record.

## Relations

The **Relations** tab is used to add representative terms, related content, or related people to your person record. 

### Representative term

!!! requirement
    There must be people taxonomy terms created to populate this field. To create a people term, navigate to [Managing Taxonomies](../taxonomies/ManagingTaxonomies.md)

 Representative terms are existing taxonomic people terms. These should reflect the name or names of the person over the course of their life. This allows the individual to be properly identified by the name or names they are known by in their community, and can help to remove distortion caused by misnamings, misspellings, or mistaken attributions. 

1. In the **Representative Term** section, select the "Select Terms" button to add an existing people term to your person record.
2. To search for specific terms, enter the term in the *Search* field and select the "Search" button.
3. Select the checkbox associated with the name(s) you want to apply to your person record.
4. Select the "Add Terms" button to add your people terms. 

![Screenshot showing the representative term section with the fields filled out and content selected.](../_embeds/placeholderscreenshot.png)

### Related content

2. In the **Related Content** section, select the "Select Content" button to add content to your person record. Related content includes anything that has a close connection to the person, including digital heritage items, dictionary words, person records, and collections. 

    - Select the *Type* dropdown field to filter content by type. Content can also be filtered by entering the name of the content in the *Title* field. Select the "Apply" button to apply these filters.
    - Select the checkbox associated with the content you want to apply to your person record.
    - Select the "Add Content" button to add your content. 

    ![Screenshot showing the related content section with the fields filled out and content selected.](../_embeds/placeholderscreenshot.png)

### Related people

1. In the **Related People** section, select the "Add Related Person" button to add a related individual to your person record. Related people is a broad field that can encompass many different types of interpersonal relationships. Some examples of relationships include family members, friends, community members, and other complex relationships.
2. Select the "Select Content" button to add another person record.
    
    - To search for a specific person record, enter the name of an individual in the *Title* field and select the "Apply" button.
    - Select the checkbox associated with the name(s) of related people you want to apply to your person record.
    - Select the "Add Content" button. 

3. In the *Relationship Type* field enter the name of the type of relationship between the individuals. This is an autocomplete field that is tied to the **Interpersonal Relationship** taxonomy terms. 
    
    - If the relationship type term already exists in the taxonomy, begin typing the term and select it from the autocomplete suggestions.
    - If the relationship term does not exist in the taxonomy, enter the full term. The new term will be added to the taxonomy when you save your person record. 
    - For more information on managing taxonomy terms, navigate to [Managing Taxonomies](../taxonomies/ManagingTaxonomies.md).

    ![Screenshot showing the relationship type field filled out with an autocomplete generated selection of taxonomy terms](../_embeds/placeholderscreenshot.png)

4. To add another related person, select the "Add Related Person" button to add additional location text boxes.
      
    - Select and drag the arrows by the location to reorder your related people if necessary.
    - To remove a related person, select the "Remove" button.

Select the "Save" button to save your person record.