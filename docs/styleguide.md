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
- Article page names should be modified versions of the [Article titles](#article-titles).
- Use CamelCase, and do not separate words in the filenames.
- Omit conjunctions, articles, and other connecting words from the filenames.
- Eg: `LocalizationTranslationOverview.md`, `CreateCollection.md`

### Image embeds

- Place all image files in the `docs/_embeds` subfolder.
- See [Image filenames](#filenames) for more information.

## Navigation menu

- Topics and articles must be referenced in the `nav` section at the end of the `mkdocs.yml` top-level file to be included in the navigation menu.
    - Articles *can* be created without including them in the navigation menu, but this is not common practice. If you do this, the site will still build, but the terminal/console will display a warning.
- Follow the established list and indent structure in place.
- Enter topic names using their full name, in title case, followed by a colon.
    - If the topic only includes a single article/page, provide the relative path to the article/page after colon.
    - If the topic includes multiple articles, provide the relative paths to the articles on indented lines below the topic.
- Article titles don't need to be provided, they are referenced in their respective markdown files.

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
    - `tags: [tag names]` - tags allow us to group pages by tagged topics, not just by their topic in the navigation menu. Tags are displayed at the top of the article page and can selected in order to view all articles with that tag. 
```
Eg:

---
pdf: false
tags:
    - media
    - content
---
```
- Here are the tags currently in use:

     - media
     - metadata
     - roundtrip
     - users
     - content 
     - about Mukurtu
     - account management
     - collections
     - comments
     - communities, cultural protocols, and categories
     - dictionary
     - digital heritage items
     - getting started
     - infrastructure
     - Local Contexts
     - look and feel
     - mapping
     - migration
     - person records
     - search
     - security
     - site maintenance
     - structure
     - taxonomies
     - translation and localization
     - user roles and responsibilities
     - workflows

### Article titles

- MUST use H1 (`# `).
- Include an empty line below title headings.
- Use title case.
- Article titles should be as short as possible, while still being clear and descriptive.
- See [Article types and titles](#article-types-and-titles) for more information on article names.
- Eg: `# Creating Communities`

### Section headings

- Start with H2 (`## `) and go down to H4 (`#### `) as needed.
- Include an empty line below section headings.
- Create sections where it is logical in the documentation structure; they are displayed on the right sidebar of the article.
- Use sentence case.
- Eg: `## Assigning community managers`

## Markdown syntax

- All articles and pages are written using Markdown syntax. Our most frequently used elements are provided here, but please reference these additional resources for more tools.
- All of the Markdown basic syntax elements are supported: <https://www.markdownguide.org/basic-syntax/>
- The Material for MkDocs theme that we use also supports additional elements: <https://squidfunk.github.io/mkdocs-material/reference/admonitions/>

### Headings

- Headings are addressed above in the [Structuring Articles and Pages section](#structuring-articles-and-pages).
- Include an empty line below all headings.

### Paragraphs and body text

- No formatting is required to wrap paragraphs. Unless text is marked as a heading or other special formatting it will be treated as body text.
- Use empty lines for line breaks.

### Blockquotes

- ??? Unsure how we will use these.

### Admonitions (call outs)

- Admonitions provide clear visual indicators that ask for more attention through use of color, icon, styling, and placement.
- They are used to highlight warnings, reminders, and other check ins.
- The available admonitions are:
    - roles "User roles"
    - tip
    - requirement
    - warning
- An admonition starts with three exclamation marks, followed by the admonition type. Indent the content of the admonition below.

```
Eg:

!!! note
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```

- To override the default title of the admonition, follow the admonition type with the desired title in double quotes.
    - You must include the "User roles" title override.

```
Eg: 

!!! note "Phasellus posuere in sem ut cursus"
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```

- There must be an empty line before and after every admonition.


### Lists

**Unordered lists (bullet points)**

- To create an unordered list, add dashes (-) in front of line items. 
    - Asterisks (*) and plus signs (+) work as well, but this documentation will use dashes.
- Indent one or more items (using tab or 4 spaces) to create a nested list.
- There must be an empty line before and after the list.

```
Eg: 

- Item
- Another item
    - Indented item

```

**Ordered (numbered) lists**

- To create an ordered list, add line items with numbers followed by periods. 
- Indent one or more items (using tab or 4 spaces) to create a nested list.
    - When creating nested lists, the indented items should use bullet points.
- There must be an empty line before and after each list.

```
Eg: 

1. Item
2. Another item
    - Indented item
```

### Emphasis

- Wrap text in single asterisks for *italics*: `*italics*`
- Wrap text in double asterisks for **bold**: `**bold**`
- Wrap text in three asterisks for ***bold and italics***: `***bold and italics***`

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

## Screenshots and images

- This documentation includes many screenshots to accompany the text. We do not anticipate using many other types of images.
- Screenshots or images are never a replacement for written information. They should never give information that is not also provided in text. Use them as an optional shortcut to understanding the information or processes.
- Always place screenshots and images BELOW their corresponding text.
- Include an empty line before and after screenshots.

### Taking good screenshots

- You can use your system's screenshot tool or a browser extension to capture screenshots.
- Screenshots should be taken with your browser zoom at 100%.
- Screenshots do not need to be the full width of your monitor.
- In general, capturing the full width of the page, instead of cropping to a more portrait orientation will look better on the site. But use good judgement.
- A screenshot of a portion of the interface should include enough visual context around the focus area to orient readers. Too narrow of a focus is not effective.
- If necessary, widen the browser window enough to include whitespace and keep things from looking cramped.
- If there is a visual difference between browsers, include representative screenshots of each (eg: Firefox and Chrome have audio players that look different).
- Save screenshots as PNG files.

### Filenames

- Image files should be short, descriptive, and include numbering to indicate their placement within an article as needed. 
- Image filenames should roughly indicate the the topic and article where they are embedded.
- Separate words with a hyphen, do not use capital letters.
- If an article includes 10 or more images, use a 2-digit numbering. Default to 2-digit numbering if unsure.
- Images should be PNG files where possible.
- Eg: `category-create-1.png`, `migration-credentials-01.png`

### Annotating screenshots

- Screenshots should be annotated/marked up to indicate the area of focus. This can be done several ways depending on what is conveyed in the screenshot.

**Arrows**

- ???

**Outlines**

- ???

**Dimming**

- ???

### Embedding image files
- The syntax to embed an image is `![Alt text for the image.](../docs/_embeds/filename-here-01.png)`
    - Alt text requirements are provided in [Alt test](#alt-text).
- Eg: `![Screenshot of the create digital heritage item form.](../docs/_embeds/create-dh-01.png)`
- Images use a lightbox tool, so any image can be clicked on to view it at full resolution.
- Images can be links
    -  ??? they need different alt text

### Alt text

- https://www.archbee.com/blog/screenshots-in-technical-documentation 
- All screenshots and images should have alt text.
- <https://www.csun.edu/universal-design-center/document-learning-tools#DescribingImages> 
- <https://intranet.birmingham.ac.uk/staff/resources/digital/web-resources/editor-resources/guidelines/accessibility/alt-text.aspx>
- ??? how to write good alt text ???

## Writing tone and style

### Article types and titles

- There are a few major article types used in this documentation. Most articles will fall into one of these types, but there may be exceptions.

**Informational articles**

- Informational articles provide an overview, explanation, or otherwise explain the core concept and purpose behind a feature or tool.
- They are typically the first article in the navigation menu for a given topic.
- Use the naming convention `Understanding _____`
- Eg: `Understanding Collections`

**Instructional articles**

- Instructional articles show how to use a feature or tool.
- They usual follow a corresponding informational article.
- Use the naming convention `[Verb] [Feature]`
- Eg: `Create a Collection`, `Upload a Media Asset`, `Edit a Cultural Protocol`

**Additional articles**

- Additional articles can cover more detailed information, technical specifications, and other topics.
- Keep titles simple.
- There is no set naming convention.
- Eg: `Vimeo Privacy Settings`, `Digital Heritage Item Metadata`

**FAQs**

- FAQs (frequently asked questions) are a specific type of article presented in a Q&A style to reflect common user questions that are not easily answerable from existing documentation.
- Use question-based titles.
- Eg: `Can the System Administrator View All Content?`

**???Other types of articles?**

### Tone and style

- The Mukurtu user base includes individuals with a wide range of technical understanding and areas of expertise. We should always try to use language that is easily understood and followed by the largest group of potential users. The following guidelines are not exhaustive.
- Based on this user interface documentation guide from Microsoft <https://learn.microsoft.com/en-us/power-platform/well-architected/experience-optimization/user-interface-content>, our writing should...
    - Be concise and scannable;
    - Be contextual and task-focused;
    - Use plain language;
    - Employ a polite and friendly tone;
    - Maintain stylistic consistency;
    - Consider and international audience;
    - Make regular use of declarative and imperative language, limited use of interrogative language, and sparing use of exclamatory language;
    - Primarily use active voice;
    - For general guidelines (especially when recommending things to avoid or error messages) use passive voice.
- Be direct.
- We should strive to provide accessible documentation to support use of screen readers and other tools...
    - Use `select` instead of `click/click on` page elements. This is more inclusive of those using screen readers and other assistive tools;
    - Avoid using `-` in text as a separator. It is fine when used in compound words and markdown syntax.;
    - Use the proper heading formats;
    - Use image alt text;
    - Used descriptive link text (eg: not "Read more")
    - Avoid other problematic or ableist language, eg: <https://arthalearning.com/accessible-and-inclusive-language-in-elearning/#/>.
- Include textual and visual examples where beneficial.
- Use specific language for different types of UI interactions <https://learn.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui>
- Use consistent stylistic indicators to communicate things like buttons, interface elements, and other features 
    - ??? ONLY in relation to the instructions/screenshots/etc on page

**Buttons**

- Indicate buttons in quotes.
- Eg: `When all information is entered, select the "save" button at the bottom of the page.`

**Interface features**

- Indicate interface features (such as page titles, page tabs, links, dropdown menus, and checkboxes) in **bold**. 
- Eg: `Select the **rights and permissions** tab.`

**Field names**

- Indicate field names and labels in *italics*.
- Eg: `The *summary* is a short descriptive field that accompanies and may help expand or disambiguate the *title*.`

**Other features**

- Indicate URLs, file paths, and bits of code in `code formatting`.
- Eg: `Navigate to your dashboard, or go directly to `/admin/dashboard`.`

**Mukurtu terms**

- Do not capitalize Mukurtu terms outside of proper nouns, titles, and headings as appropriate. 
- Eg: `community`, `cultural protocol`, `digital heritage item`, `Mukurtu CMS`, `Local Contexts`

**User roles**

- Indicate the relevant user role(s) using the ??? admonition at the start of an article, and anywhere it needs to be noted within an article.

## Video (TBD)

- ???

## GIFs (TBD)

- ???
