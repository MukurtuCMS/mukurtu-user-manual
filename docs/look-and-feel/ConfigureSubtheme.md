---
tags:
    - look and feel
---

# Configure Subtheme

!!! roles "User role"
    Drupal administrator

The most effective way to customize the look and feel of your site without having to reimplement changes is to install a subtheme. Subthemes are built off the main Mukurtu_v4 theme, and inherit the parent theme's resources while functioning like any other theme.

!!! warning 
    The instructions in this article require a degree of familiarity working with command line tools and editing code, which is not without risk. Changing your code may break your site and corrupt your data. Before following these instructions, make sure to back up your site, and confirm that you can restore from a backup.

Navigate to `\web\profiles\mukurtu\themes\mukurtu_v4`.

Create a `Themes` folder.
Create a subfolder with the name of your subtheme. For this example, we will use `subtheme1` as the name of our subtheme.
Copy all the files from the parent theme to your subtheme folder.
Rename the `mukurtu_v4.info` and `mukurtu_v4.libraries` YAML source files to `subtheme1.info` and `subtheme1.libraries`.
Open the `.info` file. Rename the **name** field to reflect the name you want to give your subtheme. 
Use the **description** field to describe your subtheme. It can be helpful to annotate which parent theme your subtheme is a child of.
In the **base theme** field, input `mukurtu_v4`.
Use the **libraries** field to annotate your subtheme. This should read `subtheme1/global-styling`.

You can use subthemes to implement changes to your font, color scheme, etc.

