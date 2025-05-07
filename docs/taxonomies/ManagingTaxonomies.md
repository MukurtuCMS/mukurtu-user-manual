---
tags:
    - taxonomies
    - categories
---

# Managing Taxonomies

!!! roles "User roles"

    Mukurtu administrator

There may be a need to manage or clean up taxonomy terms. Most commonly this happens when users mis-enter a term (eg: typing "baskey" when they meant "basket"), or enter a similar term (eg: "basket" instead of "baskets"), though there are many other situations where this may be necessary.

## Accessing a taxonomy

All taxonomies can be accessed at `/admin/structure/taxonomy`

1. From the "Manage" menu, select "Structure".
2. From the list, select "Taxonomy".

    SCREENSHOT

3. To view a taxonomy, on the far right of the its row, select "List terms".

    SCREENSHOT

4. From here, you can edit individual terms, or merge terms to together.

    SCREENSHOT

## Editing taxonomy terms

You may want to edit a taxonomy term. For example, you notice a spelling error.

!!! tip

    When a taxonomy term is edited, those edits appear across all site content using the term. No need to manually edit each piece of content.

1. From the appropriate taxonomy list, identify the relevant term, and on the far right of its row, select "Edit".

    SCREENSHOT

2. From here you can edit the term name, and any other fields as necessary. See INSERT LINK TO "ADDING TAXONOMY TERMS" for more information on available fields.

    SCREENSHOT

3. When done, select "Save" at the bottom of the page.

    SCREENSHOT

4. The taxonomy list will load and a confirmation message is displayed.

    SCREENSHOT


## Deleting taxonomy terms

You may want to delete a taxonomy term. For example, you entered a term in the wrong field, or simply choose to no longer use that term.

!!! warning

    If you delete a term, it will be removed from all content where it is used.

1. From the appropriate taxonomy list, identify the relevant term, and on the far right of its row, select "Delete".

    SCREENSHOT

2. From the warning message select "Delete".

    SCREENSHOT

3. The term is deleted and a confirmation message is displayed.

    SCREENSHOT

## Merging taxonomy terms

You may want to merge multiple taxonomy terms together. For example, different users have used "baskets" and "basket making" as *keywords*, and you want to combine them into a more general "basketry" term.

!!! tip

    When a taxonomy term is edited, those edits appear across all site content using the term. No need to manually edit each piece of content.

1. From the appropriate taxonomy list, below the taxonomy name, select "Merge".

    SCREENSHOT

2. To choose the terms you want to merge together, select them with the available checkboxes, then select "Save" at the bottom of the page.
    - To merge multiple terms into a new target term, select all terms to merge here. The new target term will be created on the next page.
    - To merge one or more terms into another existing target term, select them here. The target term will be selected on the next page, do not select it now.

    SCREENSHOT

3. Either enter a new target term, or select an existing target term, then select "Merge terms" at the bottom of the page.
    - To merge the selected terms into a new target term, enter it in the "New term" field.
    - To merge the selected term(s) into an existing target term, select it from the "Existing term" list.   

    SCREENSHOT

4. A confirmation message will be displayed. If the information is correct, select "Confirm merge" at the bottom of the page.

    SCREENSHOT

5. The page will reload and a confirmation is displayed.

    SCREENSHOT

## Taxonomy term merge management

When taxonomy terms are merged, the system keeps a record of the merges, generates rules, and automatically applies those merge rules if those same terms are entered again later. This is done with the "Term Merge Manager" module.

For example:

1. You merge the *keywords* "baskets" and "basket making" into a more general "basketry" term.
2. The system generates two rules from this:
    - "Baskets" should always be replaced with "basketry", and
    - "Basket making" should always be replaced with "basketry".
3. The next time a user enters "baskets" or "basket making" into a *keywords* field, the system automatically replaces them with the term "basketry".

These rules can be edited and removed if needed. For example, you may decide in the future that you DO want "basketry" and "baskets" to be separate *keywords*.
