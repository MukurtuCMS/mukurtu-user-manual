---
pdf: false
---

# Mukurtu user manual style guide

## Folders and files
- All of the articles and image embeds are located in the `docs` folder in this repository.
    - ***Do not*** edit anything in the `docs/_static` subfolder, or the `requirements.txt` document.
- ***Do not*** edit the `site` or `venv` folders.
- ***Do not*** edit any of the following top-level files: `.gitattributes`, `.gitignore`, `.readthedocs.yml`, `README.md`
- In the `mkdocs.yml` file, ***only*** edit the `nav` section at the end of the document (this controls the navigation menu). ***Do not*** make any other changes to this document.

### Topic folders
- Each topic has a subfolder in the `docs` directory.
- Topic folder names should be short and distinct. Longer names can be provided in the navigation menu.
- Separate words with a hyphen, do not use capital letters.
- Eg: `digital-heritage-items`, `collections`, `local-contexts`

### Article pages
- Place all article pages in the subfolder corresponding to their primary topic. Some articles may touch on multiple topics, this will be indicated with tags.
- All article pages must end with the `.md` (markdown) extension.
- Article page names should be descriptive.
- Use CamelCase, and do not separate words.
- Omit conjunctions, articles, and other connecting words.
- Eg: `LocalizationTranslationOverview.md`, `CreateCollection.md`

### Image embeds
- Place all image files in the `docs/_embeds` subfolder.
- Image files should be short, descriptive, and include numbering to indicate their placement within an article as needed. 
- Image filenames should roughly indicate the the topic and article where they are embedded.
- Separate words with a hyphen, do not use capital letters.
- If an article includes 10 or more images, use a 2-digit numbering.
- Images should be PNG files where possible.
- Eg: `category-create-1.png`, `migration-credentials-01.png`
- For more information on formatting images and embedding them in articles, see the formatting sections of this guide.

## Navigation menu
- Topics and articles must be referenced in the `nav` section at the end of the `mkdocs.yml` top-level file to be included in the navigation menu.
    - Articles *can* be created without including them in the navigation menu, but this is not common practice. If you do this, the site will still build, but the terminal/console will display a warning.
- Follow the established list and indent structure in place.
- Enter topic names using their full name, in title case, followed by a colon.
- If the topic only includes a single article/page, provide the relative path to the article/page after colon.
- If the topic includes multiple articles, provide the relative paths to the articles on indented lines below the topic.

```
Eg: 

  nav:
    - Home: index.md
    - Collections:
      - collections/CreateCollection.md 
      - collections/UnderstandingCollections.md
    - Localization and Translation:
      - localization-translation/LocalizationTranslationOverview.md 
```

## Formatting 

### Navigation sections (topics)
- Use title case.
- Eg: `Communities and Cultural Protocols`

### Article titles
- MUST use H1 (`# `).
- Use title case.
- Eg: `# Creating Communities`

### Section headings
- Start with H2 (`## `) and go down to H4 (`#### `) as needed.
- Create sections where it is logical in the documentation structure; they will appear in the left navigation of the documentation. 
- Use sentence case.
- Eg: `## Assigning community managers`

### Mukurtu terms
- Do not capitalize Mukurtu terms outside of titles and headings as appropriate.
- Eg: community, cultural protocol, digital heritage item.

### Buttons
- Indicate buttons in quotes.
- Eg: `"Save"`

### Interface features
- Indicate interface features (such as page titles, page tabs, links, dropdown menus, and checkboxes) in **bold**. 

### Field names
- Indicate field names and labels in *italics*.

### Other features
- Indicate URLs, file paths, and bits of code in `code formatting` (text between backticks ``).

### Links

**Internal links**
- Should be composed as relative to the current file. 
- They will look something like `../Plugins/CSV_Import.md` if you are linking to a page that sits within a folder, or `../Admin/Users.md#add-a-user` if you are linking to a section of a page. 
- Do not forget the `.md` part of the page.

**External links**
- Links to external websites require the full URL as well as the addition of "{target=_blank}" after the link syntax.
- Eg: `[create a new issue](https://github.com/omeka/classic-enduser/issues){target=_blank}`.

### Images
- Images should never give information that is not provided in the text (or in the image alt text and title). No one with vision problems should be missing out. Think of images as a shortcut, not the only route, to understanding how to do something. 

**Location**
- Place all images in the `embed` directory. 

**Filenames**
- Name images clearly, starting with an indicator of the relevant page, and use an underscore to separate out the image's purpose (for example, `items_addItem.png`).
- - CamelCase or hyphen-separated?
- Number steps.

**Alt text**
All images should have alt text. A title can also be supplied if having some pop-up text would be useful to readers. An image entered in Markdown looks like this:

```
Some text ends here.

![Alt text for the image goes here.](../doc_files/animage_pathGoesHere.png "An optional title which will appear when a user mouses over the image.")

More text picks up here.
```

The maximum display width of an image in the user manuals currently is around 1300px (actually 1296px). A screenshot of the full Omeka Classic interface (public or admin side) should be large. Images can be saved larger (up to 2000px wide) so that readers can open them in new tabs and inspect them in full-scale detail if desired. 

A screenshot of a portion of the interface, such as the left-hand navigation, should appear at full scale for maximum readability. Currently, Omeka Classic has a left-side menu-bar width of about 200px, and a main content width of about 1040px, on a 1920x1080 screen. Expand the browser window wide enough to add some whitespace and keep things from looking cramped, but screenshots do not need to be the full width of your monitor.

**Linking to full-size image**
- `[![alt text](path to image)](path to image)`

**Taking screenshots**
- Use PNG images.

**Image markup**

*Arrows*

*Circles?*


## Writing
- Include admonitions and call-outs. Especially when a external step is required.
- Include examples.
- Separate high level info vs how to use.

- "Create a ____"
- 