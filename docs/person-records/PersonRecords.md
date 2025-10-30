---
tags:
    - content
    - person records
    - taxonomy
---
# Create Person Records

!!! roles "User roles"
    Protocol steward, contributor

Person Records allow for rich biographical records to be integrated into Mukurtu CMS. Person records can include birth and death dates as well as custom text and media sections. They can also identify relationships between people, and aggregate all digital heritage items where a person is referenced. They can also act as authority records, referencing all the names that a person is known by. Follow the instructions below to create a person record.

!!! requirement
    You must configure the person records settings before creating new person records. Navigate to the [Configure Person Record Settings](person-records\ConfigurePersonRecord.md) article for instructions. 

From any of your **Dashboard** or **Add Content** links, select **Person Record**.

![Screenshot of the Mukurtu landing page with the Dashboard links highlighted and the Add Content + highlighted, as well as the Create Content dropdown with Person Record highlighted.](../_embeds/person1.png)

## Mukurtu Essentials

### Name

Enter the person's name as they should be primarily identified in the *Name* field. Names can be formatted as `Last, First, Middle`, `Last, First (Nickname)`, `Family name, Given name`, or any other format that makes sense for your community.

- This is a required field.

### Cultural protocols

Use the checkboxes to apply cultural protocols to your digital heritage item. 

- This is a required field.

### Sharing settings

Use the checkboxes to select a **Sharing setting**. Sharing setting has two options: you can select **Any** or **All**. 

- Any is the less restrictive setting as it means that the content can be shared with people belonging to any one or more of the protocols selected. 
- All is more restrictive as users must belong to all the selected protocols to view the digital heritage item. 
- This is a required field.

![Screenshot with the sharing setting and cultural protocols selected.](../_embeds/placeholderscreenshot.png)

### Other names

People may be identified by multiple names, monikers, or identities, sometimes with inconsistent spellings across different content. The other names field is used to aggregate and display all content where the person is identified by connecting those disparate names.

This is dependant on proper person record settings configuration. If there are no terms displayed here, either you have not properly configured the person record settings, or there are no matching names in your configured fields. Review the [Configure Person Record Settings](ConfigurePersonRecord.md) article for instructions.

!!! requirement
    There must be enabled person taxonomy terms created to populate this field. To create a creator, contributor, or people term, navigate to [Managing Taxonomies](../taxonomies/ManagingTaxonomies.md)

1. In the **Other Names** section, select the "Select Terms" button to add an existing term to your person record.
   
    !!! tip 
        You can search for specific terms using the Search field.

2. Select the checkbox beside all the terms you wish to include, then scroll down and select "Add Terms".

![Screenshot showing the other names section with the fields filled out and content selected.](../_embeds/person2.png)

3. Select "Finished" to add the terms to your person record. To remove terms from your record, select the **Delete** icon to the top right of each term from the modal or the field. 

![Screenshot of the select terms modal with terms selected. The delete icon and finished button are both highlighted.](../_embeds/person3.png)

### Media assets

Media assets are a key element of most person records, though they are not required. Supported media types are images, documents, video, audio, and embed code. Person records can include more than one media asset, and each media asset can be a different media type. Media assets can be assigned a different cultural protocol from the person record to allow differential access to the media assets and metadata. For instructions on how to add a media asset, refer to the [Create Media Assets](/docs/media/CreateMediaAssets.md) article.

- You can add multiple media assets by selecting more than one media asset from the media modal. 
- To reorder your media assets, select your media assets and drag them into the order you prefer.

![Screenshot with a media asset applied.](../_embeds/person4.png)

### Date fields

1.  In the **Date Born** section enter the date the person was born. Enter the year and, if known, select the month and day.
2. In the **Date Died** section enter the date the person died. Enter the year and, if known, select the month and day.
3. Use the slider to indicate whether the person is **Deceased**. This field informs the deceased person media content warning. For more information on this and other media content warnings, please see the [Media Content Warnings](../media/MediaContentWarnings.md) article.

![Screenshot of the date and deceased fields with information filled in to indicate the dates the person was born and died, and that the individual is deceased.](../_embeds/placeholderscreenshot.png)

## Biography

This is where you can provide interpersonal relationships and biographical information for your person record. 

### Related people

!!! requirement
    Related person records must have already been created in order to be added to the related people section. 

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

### Biography sections

1. Under the **Biography Sections**, enter the title of the biographical information in the *Title* field. 
2. Use the *Body* field to provide a longer biographical sketch for your person record. This field enables a broader narrative that can include a written biography, audio recordings, video recordings, images, or any other supportive information for your person record. This is a full HTML field that supports text, audio, images, and video media assets.
3. Select the "Add Formatted Text with Title" button to add an additional biography section. 

    !!! tip
        Adding multiple biography sections allows users a more clearly delineated way to provide multiple people's perspectives on the individual's life or separate different aspects of their life, activities, or work.

![Screenshot with the text sections and biographical information sections filled in with example text.](../_embeds/placeholderscreenshot.png)

You can save your person record at this point, or return to the top of your page to select the **Mukurtu Essentials**, **Relations**, or **Additional Fields** tabs to add more context to your person record.

## Additional Fields

The **Additional Fields** tab is used to add keywords, mapping and location information, and Local Contexts labels and notices to your person record.

### Keywords

In the **Keywords** section, add keywords that would help users find the person record. This may include significant events or organizations they were a part of, or other related terms. Keywords provide an additional way to categorize your content. In general, 3-5 keywords are recommended to make it easier for users to search and retrieve content. 
   
1. Select the "Add another item" button to add additional keyword text boxes.
2. Select and drag the arrows by the keyword to reorder your keywords if necessary.
3. To remove a keyword, select the "Remove" button.

### Locations

1. Use the **Map Points** Leaflet map to enter one or more geographic locations for your person record. This can be an area that the person lived in, that they were associated with, or any other geographic location. Use the buttons on the right to enter points, paths, rectangles, or polyons to your map. You can also add markers to your map by uploading GeoJSON shapes. For more information on how to use the **Map Points** Leaflet map, visit [Create Map Points](../map-points/CreateMapPoints.md)
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

Select the "Save" button to save your person record.

## Related content

The **Related content** tab is used to add related content to your person record. 

### Related content

!!! tip
    If properly configured, the site will auto-aggregate content related to this person. In most cases this field will not be used.

In the **Related Content** section, select the "Select Content" button to add content to your person record. Related content includes anything that has a close connection to the person, including digital heritage items, dictionary words, person records, and collections. 

1. Select the *Type* dropdown field to filter content by type. Content can also be filtered by entering the name of the content in the *Title* field. Select the "Apply" button to apply these filters.
2. Select the checkbox associated with the content you want to apply to your person record.
3. Select the "Add Content" button to add your content. 

    ![Screenshot showing the related content section with the fields filled out and content selected.](../_embeds/placeholderscreenshot.png)

## Browse person records

To browse person records, navigate to **Browse** or go directly to `/browse`. To filter by person records, navigate to the **Content type** header on the right-hand side of the page and select the checkbox beside *Person*. 

![Screenshot showing where the content type header and person checkbox are on the browse content page.](../_embeds/placeholderscreenshot.png)