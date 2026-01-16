---
tags:
    - taxonomies
    - categories
---

# Managing Taxonomies

!!! roles "User roles"

    Administrator, Mukurtu manager

There may be a need to manage or clean up taxonomy terms. Most commonly this happens when users mis-enter a term (eg: typing "baskey" when they meant "basket"), or enter a similar term (eg: "basket" instead of "baskets"), though there are many other situations where this may be necessary.

## Accessing a taxonomy

1. All taxonomies can be accessed at `/admin/structure/taxonomy`

    ![The entire web browswer showing the taxonomies list. The URL with /admin/strucutre/taxonomy is higlighted](../_embeds/manage-tax-01.png)

2. Alternatively, from the dashboard, scroll down to the **Taxonomies** section and select "Manage Taxonomies."

    ![The dashboard with "Manage Taxonomies highlighted"](../_embeds/manage-tax-1.1.png)

3. To view the terms in a taxonomy, from the far right of the row select "List terms". From here, you can edit individual terms, or merge terms to together.
   
    ![The taxonomy page with "list terms" highlighted](../_embeds/manage-tax-02.png)

Here are some terms created in the *keyword* taxonomy

![The keyword taxonomy list with terms "food," and "recipes"](../_embeds/manage-tax-03.png)

## Add a taxonomy term

1. To add a new term, select "Add Term"

    ![The term list with the +Add term button highlighted](../_embeds/manage-tax-18.png)

2. Add the term you would like to use, any additional metadata as needed, and select "Save."

    ![The add term form filled out. The save button is highlighted](../_embeds/manage-tax-19.png)

3. A page will reload and a success message will be displayed

    ![The add term form with a success message displayed](../_embeds/manage-tax-20.png)

## Edit taxonomy terms

There are several reasons you may want to edit a taxonomy term. Eg: spelling errors, updating terms.

!!! tip

    When a taxonomy term is edited, those edits apply to all content using the term. There is no need to manually edit each piece of content.

1. Identify the relevant term from the appropriate taxonomy list. From the far right of its row select "Edit".

    ![The keyword taxonomy list with the edit button highlighted for "food"](../_embeds/manage-tax-04.png)

2. From here you can edit the term name, and any other fields as necessary. When done, select "Save" at the top of the page.

    ![The "food" taxonomy term has been changed to "cuisine". The "save" button is highlighted](../_embeds/manage-tax-05.png)

4. The taxonomy list will load and a confirmation message is displayed.

    ![The taxonomy list with a confirmation message displayed](../_embeds/manage-tax-06.png)

## Delete taxonomy terms

There are several reasons you may want to delete a taxonomy term. For example, you entered a term in the wrong field, or simply choose to no longer use that term.

!!! warning

    If you delete a term, it will be removed from all content where it is used.

1. Identify the relevant term from the appropriate taxonomy list. From the far right of its row, select "Delete" from the dropdown menu.

    ![Taxonomy term with delete button highlighted](../_embeds/manage-tax-07.png)

2. From the warning message select "Delete".

    ![The warning message with Delete and Cancel buttons](../_embeds/manage-tax-08.png)

3. The term is deleted and a confirmation message is displayed.

    ![The taxonomy list with a confirmation message displayed.](../_embeds/manage-tax-09.png)

## Merge taxonomy terms

You may want to merge multiple taxonomy terms together. For example, different users have used "baskets" and "basket making" as *keywords*, and you want to combine them into a more general "basketry" term.

!!! tip

    When a taxonomy term is edited, those edits apply to all content using the term. There is no need to manually edit each piece of content.

1. From the appropriate taxonomy list, below the taxonomy name, select "Merge".

    ![The taxonomy list with the "mergeʻ button highlighted](../_embeds/manage-tax-10.png)

2. To choose the terms you want to merge together, use the checkboxes to select them. Select "Next" at the top of the page.
    - To merge multiple terms into a new target term, select all terms to merge here. The new target term will be created on the next page.
    - To merge one or more terms into another existing target term, select them here. The target term will be selected on the next page, do not select it now.

    ![The keyword taxonomy page listing all terms. Some terms are selected for merging.](../_embeds/manage-tax-11.png)

3. Either enter a new target term or select an existing target term. Select "Merge terms" at the bottom of the page.
    - To merge the selected terms into a new target term, enter it in the "New term" field.
    - To merge the selected term(s) into an existing target term, select it from the "Existing term" list.   

    ![The Select target term form displaying the new term field and existing term drop down menu.](../_embeds/manage-tax-12.png)

4. A confirmation message will be displayed. If the information is correct, select "Confirm merge" at the top of the page.

    ![The confirmation message. "Confirm merge" is highlighted.](../_embeds/manage-tax-13.png)

5. The taxonomy list will load and a confirmation message will display.

    ![The merge page reloaded with the keyword list. The taxonomy terms have been merged.](../_embeds/manage-tax-14.png)

## Taxonomy term merge management

When taxonomy terms are merged, the system keeps a record of the merges, generates rules, and automatically applies those merge rules if those same terms are entered again later. This is done with the "Term Merge Manager" module.

For example:

1. You merge the *keywords* "baskets" and "basket making" into a more general "basketry" term.
2. The system generates two rules from this:
    - "Baskets" should always be replaced with "basketry", and
    - "Basket making" should always be replaced with "basketry".
3. The next time a user enters "baskets" or "basket making" into a *keywords* field, the system automatically replaces them with the term "basketry".

These rules can be edited and removed if needed. For example, you may decide in the future that you DO want "basketry" and "baskets" to be separate *keywords*. 

1. As an administrator, you can manage these rules at `admin/structure/term_merge_from`

Alternatively, select the **Structure** menu in the left hand sidebar menu and select **Term Merge from list** near the bottom of the menu. 

![The structure menu icon - three squares layered on top of each other - which opens the structure menu is highlighted. The "merge term from list" menu item is also highlighted.](../_embeds/manage-tax-15.png)    

This can also be accessed through the dashboard in the **Taxonomies** section.
![The dashboard with "Manage taxonomy term merge list" highlighted](../_embeds/manage-tax-21.png)

In the "Name" column is a list of terms that will automatically be replaced when used in content. In this example, "Basket making" and "Baskets" will be changed to "Basketry" when used.

2. To allow for "baskets" to be a separate keyword again, identify the "Baskets" rule and select "delete".

    ![The term "merge from list" with "delete" highlighted for the "Baskets" rule](../_embeds/manage-tax-16.png)

2. Select "Delete" again on the confirmation message. 

3. "Baskets" can now be used as a keyword in content and will not be replaced by "Basketry."

    ![A digital heritage item showing the keyword "baskets" in the metadata](../_embeds/manage-tax-17.png)

