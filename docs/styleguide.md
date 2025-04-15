---
pdf: false
---

# Mukurtu User Manual Style Guide

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
- Articles titles don't need to be provided, they are referenced in their respective markdown files.

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

## Structuring articles and pages

### Meta tags
- Articles and pages may include meta tags in the front matter of the document, before the title, which controls how the page renders and interacts with various plugins.
- These tags are placed within two rows of three hyphens (example below).
- At this time, the meta tags we use are:
    - `pdf: false` - if the page should nto generate a PDF for download.
    - `tags: [tag names]` - tags allow us to group pages by tagged topics, not just by their topic in the navigation menu. Tags are displayed at the top of the article page and can selected in order to view all articles with that tag. The tag(s) must be included in the tags section of the `mkdocs.yml` document before they can referenced in articles.

```
Eg:

---
pdf: false
tags:
    - media
    - content
---
```

### Article titles
- MUST use H1 (`# `).
- Use title case.
- Eg: `# Creating Communities`
- Article titles should be as short as possible, while still being clear and descriptive.

### Section headings
- Start with H2 (`## `) and go down to H4 (`#### `) as needed.
- Create sections where it is logical in the documentation structure; they are displayed on the right sidebar of the article.
- Use sentence case.
- Eg: `## Assigning community managers`

## Markdown syntax
- All articles and pages are written using Markdown syntax. Our most frequently used elements are provided here, but please reference these additional resources for more tools.
- All of the Markdown basic syntax elements are supported: <https://www.markdownguide.org/basic-syntax/>
- The Material for MkDocs theme that we use also supports additional elements: <https://squidfunk.github.io/mkdocs-material/reference/admonitions/>

### Headings
- Headings are addressed above in the [Structuring Articles and Pages section](#structuring-articles-and-pages).

### Paragraphs and body text
- No formatting is required to wrap paragraphs. Unless text is marked as a heading or other special formatting it will be treated as body text.
- Use empty lines for line breaks.

### Blockquotes
- Unsure how we will use these.

### Admonitions (call outs)
- Admonitions provide clear visual indicators that ask for more attention through use of color, icon, styling, and placement.
- They are used to highlight warnings, reminders, and other check ins.
- The available admonitions are:
    - note
    - abstract
    - info
    - tip
    - success
    - question
    - warning
    - failure
    - danger
    - bug
    - example
    - quote
- An admonition starts with three exclamation marks, followed by the admonition type. Leave one empty line, then indent the content of the admonition.
```
!!! note

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```
- To override the default title of the admonition, follow the admonition type with the desired title in double quotes.
```
!!! note "Phasellus posuere in sem ut cursus"

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```

### Lists
**Unordered lists (bullet points**)

- To create an unordered list, add dashes (-) in front of line items. 
    - Asterisks (*) and plus signs (+) work as well, but this documentation will use dashes.
- Indent one or more items (using tab or 4 spaces) to create a nested list.
```
Eg: 
- Item
- Another item
    - Indented item
```

**Ordered (numbered) lists**
- To create an ordered list, add line items with numbers followed by periods. 
- Indent one or more items (using tab or 4 spaces) to create a nested list.
```
Eg: 
1. Item
2. Another item
    a. Indented item
```

### Emphasis
- Wrap text in single asterisks for italics: `*italics*`
- Wrap text in double asterisks for bold: `**bold**`
- Wrap text in three asterisks for bold and italics: `***bold and italics***`

### Code formatting
- Code formatting prevents the site from rendering the markdown code, so it's useful if you want to show how to format text. It's used a lot in this style guide!
- It can also be useful for indicating code, or other code-like elements.
- Wrap text in single backticks: `` (text would go between those)
- To wrap multiple lines, place three backticks on the line above, and three backticks on the line below.

### Links
**Internal links**

- Internal links are used to link to other articles and pages with this documentation.
- They are paths relative to the current article.
- A link to an article in ***a different topic folder*** will look like `[Article Name](../[topic-folder]/[ArticleName])` 
- A link to an article in ***the same topic folder*** will look like `[Article Name](ArticleName)`
- You can also link to a section within another article by adding the modified heading to the article filename (replace spaces with hyphens and convert all to lowercase) `[Article Name](../[topic-folder]/[ArticleName#section-heading])`
- And finally you link to a section within the current article `[Section name](#section-heading)`
- Eg:
    - Article in a different topic folder: `[Create a Collection](../collections/CreateCollection)`
    - Article in the same topic folder: `[Create a Collection](CreateCollection)`
    - Section within an article: `[Steps to create a collection](../collections/CreateCollection#steps-to-create-a-collection)`
    - Section within the current article: `Steps to create a collection](#steps-to-create-a-collection)`

**External links**

- External links are used to link out to other websites and sometimes email address.
- External links need to include a complete URL. Email addresses do not require the complete `mailto:` format that is used in HTML markup.
- They should include the `{target=_blank}` attribute after the link syntax so that they open in a new tab or window (dependent on the user's browser settings). Email addresses don't require this attribute.
- They can be created two ways:
    1. To quickly turn a URL into a link, enclose it in angle brackets: `<https://mukurtu.org>`, `<https://mukurtu.org>{target=_blank}` or `<support@mukurutu.org>`
    2. To include a title, include the text/title in square brackets, followed by the URL in round brackets: `[Mukurtu CMS](https://mukurtu.org){target=_blank}`

## Images
- Images should never give information that is not provided in the text (or in the image alt text and title). No one with vision problems should be missing out. Think of images as a shortcut, not the only route, to understanding how to do something. 

**Alt text**
All images should have alt text. A title can also be supplied if having some pop-up text would be useful to readers. An image entered in Markdown looks like this:

`![Alt text for the image goes here.](../doc_files/animage_pathGoesHere.png "An optional title which will appear when a user mouses over the image.")`

The maximum display width of an image in the user manuals currently is around 1300px (actually 1296px). A screenshot of the full Omeka Classic interface (public or admin side) should be large. Images can be saved larger (up to 2000px wide) so that readers can open them in new tabs and inspect them in full-scale detail if desired. 

A screenshot of a portion of the interface, such as the left-hand navigation, should appear at full scale for maximum readability. Currently, Omeka Classic has a left-side menu-bar width of about 200px, and a main content width of about 1040px, on a 1920x1080 screen. Expand the browser window wide enough to add some whitespace and keep things from looking cramped, but screenshots do not need to be the full width of your monitor.

**Linking to full-size image**
- `[![alt text](path to image)](path to image)`

**Taking screenshots**
- Use PNG images.

**Image markup**

*Arrows*

*Circles?*


## Writing, tone, and style.
- Include admonitions and call-outs. Especially when a external step is required.
- Include examples.
- Separate high level info vs how to use.

- "Create a ____"



### Buttons
- Indicate buttons in quotes.
- Eg: `"Save"`

### Interface features
- Indicate interface features (such as page titles, page tabs, links, dropdown menus, and checkboxes) in **bold**. 

### Field names
- Indicate field names and labels in *italics*.

### Other features
- Indicate URLs, file paths, and bits of code in `code formatting` (text between backticks ``).

!!! info "Mukurtu terms"
    Do not capitalize Mukurtu terms outside of proper nouns, titles, and headings as appropriate. Eg: community, cultural protocol, digital heritage item, Mukurtu CMS, Local Contexts