---
tags:
    - multilingual
    - look and feel
---

# Configure Font

!!! roles "User role"
    Drupal admin

The primary font on Mukurtu CMS is BC Sans, which was selected for its wide support of Indigenous languages. If your site requires a custom font, you can update your font from code.

!!! warning 
    The instructions in this article require a degree of familiarity working with command line tools and editing code, which is not without risk. Changing your code may break your site and corrupt your data. Before following these instructions, make sure to back up your site, and confirm that you can restore from a backup.

If you would like to add other fonts to your theme, simply download the appropriate font files (WOFF and WOFF2 generally, though TTF is also supported) to the fonts folder in the theme, and update the relative path as needed. If a serif font is required, users should assess [First Nations Unicode Font](https://cis.arts.ubc.ca/community/first-nations-unicode-font/) from the University of British Columbia, which seems similar to BC Sans in its support of Indigenous languages. Follow the instructions below to add a font from your code source to the Mukurtu 4 and Gin (admin) themes.

!!! tip
    You can convert your chosen font to WOFF or WOFF2 format using [https://cloudconvert.com/](https://cloudconvert.com/) or any other conversion tool. Download your new file and save it in a place that is easily accessible.

## Configure Mukurtu 4 theme font

1. Select your font file. 
2. Open your file directory and navigate to `\mukurtu\themes\mukurtu_v4\fonts`. 
3. Drop your font file into the fonts folder.

    ![Screenshot of the fonts folder with the First Nations Unicode fonts included and highlighted.](../_embeds/font15.png)

4. Navigate to `\mukurtu\themes\mukurtu_v4\components\00-base\typography`.
5. Select the `_fonts.scss`file. You may choose to edit this in your browser or your preferred text editor. 
6. Edit the .scss file to reflect your chosen fonts.

    ![Screenshot of the updated _fonts.scss file with the fonts updated.](../_embeds/font16.png)

7. Save this file to update your fonts. 

## Configure Gin (admin) theme font

1. Select your font file. 
2. Open your file directory and navigate to `\themes\contrib\gin\dist\media\font`. 
3. Drop your font file into the fonts folder.

    ![Screenshot of the fonts folder with the First Nations Unicode fonts included and highlighted.](../_embeds/font17.png)

4. Navigate to `\themes\contrib\gin\dist\css\theme`.
5. Select the `_font.css` file. You may choose to edit this in your browser or your preferred text editor. 
6. Edit line 9 of the .css file to reflect your chosen fonts.

    ![Screenshot of the updated _fonts.scss file with the fonts updated.](../_embeds/font18.png)

7. Save this file to update your fonts. 