---
tags:
    - site settings
    - documentation
---

# Configure Citation Field Templates

!!! Roles "User roles" 
    Drupal administrator, Mukurtu manager

You can include recommended citation templates for your content in Mukurtu CMS to appear on content pages. To start configuring your citation templates, navigate to the **Site settings** section of the Dashboard and select the **Citation formats and default image** link, or go directly to `/admin/config/mukurtu/settings`.

## Sample citation formats

Included below are some common citation formats that you can use for your content. You can also create your own citation format or modify these so that they are appropriate for the content on your site. The citation formats that we are basing these examples on are:

- APA: [APA Formatting and Style Guide (7th Edition) from Purdue OWL](https://owl.purdue.edu/owl/research_and_citation/apa_style/apa_formatting_and_style_guide/in_text_citations_the_basics.html)
- Chicago: [The Chicago Manual of Style Online](https://www.chicagomanualofstyle.org/home.html)
- MLA: [MLA General Formatting and Style Guide from Purdue OWL](https://owl.purdue.edu/owl/research_and_citation/mla_style/mla_formatting_and_style_guide/mla_general_format.html)

### Collection

- APA: `Community, Cultural Protocol. Collection Title. Website name. URL.`
- Chicago: `Collection name. Source. Website name. URL.`
- MLA: `Collection name. Source. Website name. URL.` 

### Dictionary words

- APA: `Contributor's Lastname, Firstname. Original date. Word. In [Website name] [Language] Dictionary. Website or organization name. URL.`
- Chicago: `[Website name] [Language] Dictionary, s.v. "Word", last modified [date if known], URL .`
- MLA: `Word. [Website name] [Language] Dictionary, URL.`

### Digital Heritage items

- APA: `Creator's Lastname, Firstname. Title. Original date. Website name, URL.`
- Chicago: `Creator's Lastname, Firstname. Title. Contributor(s). Publisher. Original date. Format, running time (for audio or video files; only use if applicable). URL .`
- MLA: `Creator's Lastname, Firstname. Title. Publisher, Original date, URL.`

### Person records

- APA: `Name. Biography section Title. Website name. URL.`
- Chicago: `Community, Cultural Protocol. Name. "Biography section Title". Website name. URL.`
- MLA: `Name. Biography section Title. Website name. URL.`

### Word lists

- APA: `Community, Cultural Protocol. Word list name, Language. Website name. URL.`
- Chicago: `Word list name, Language. Source. Website name. URL.`
- MLA: `Word list name, Language. Source. Website name. URL.` 

## Configuring templates with tokens

Mukurtu CMS allows you to configure the citation field templates for all content types using tokens. Tokens act as in-text placeholders with contextual values that allow the content to auto-generate a specific citation. 

!!! tip
    Tokens are only available for Drupal fields. 

1. Navigate to the **Citation Field Templates** section of the page and select the dropdown to open the section.

    ![The Mukurtu Settings page with the Citation Field Templates dropdown section highlighted.](../_embeds/citation1.png)

2. Under any citation template field, select the **Browse available tokens** to browse pre-set tokens.

    ![Screenshot of the Browse available tokens modal link highlighted.](../_embeds/citation2.png)
    
    !!! warning
        When adding tokens to your site, use the `current-site` or `current-date` tokens. Use of the `node` tokens has the ability to break your site. 

3. Select the pre-set tokens you wish to include in your citation. These can include tokens referencing title, date, URL, or other fields.

    ![Screenshot of the Browse tokens modal with the current-site:title option highlighted.](../_embeds/citation3.png)

4. Select the "Save Configuration" button to save your citation template.

    ![Screenshot of the citation field page with the save configuration button highlighted.](../_embeds/citation9.png)

5. When users browse your site's digital heritage items, the Citation field will populate with the citation template, including the auto-generated metadata from the tokens. 

    ![Screenshot of the citation field on a digital heritage item.](../_embeds/citation8.png)

