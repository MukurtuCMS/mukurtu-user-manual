---
tags:
    - local contexts
---

# Convert Legacy TK Labels to Hub Labels

!!! roles "User roles"
    Administrator, Mukurtu manager

Move content off legacy Traditional Knowledge (TK) Labels and notices migrated from Mukurtu 3 and onto real Local Contexts Hub projects, labels, and notices, so they can be managed like any other label going forward.

!!! tip
    To learn more about legacy labels, see [Understanding Legacy Traditional Knowledge Labels](UnderstandingLegacyTKLabels.md).

## Prerequisites

- A real Local Contexts Hub project already added to the site, community, or protocol you're converting. See [Manage Local Contexts Projects](ManageLocalContextsProjects.md).

## Reassign a legacy project

This conversion tool maps a legacy project's labels and notices to a real Hub project's labels and notices, then rewrites the affected content. You don't need to map everything at once: any labels or notices you leave unmapped stay on their content untouched, and you can run the tool again later to map more.

1. From the Mukurtu dashboard, select **Remap Legacy Projects**. For a community or protocol, navigate to its page and select the **Remap Legacy Projects** tab instead.
2. Select the legacy project you want to reassign, and the target Hub project you want to reassign it to.
3. Select the "Next: Map Labels" button.

    ![The Reassign legacy Local Contexts project step with a legacy project and a target Hub project selected.](../_embeds/convert-legacy-tk-labels-01.png)

4. On the mapping step, map each legacy label or notice to its real equivalent on the target project, or leave it set to "— Skip (leave unmapped) —". This step is optional; select the "Preview" button when you're done.

    ![The mapping step with two legacy labels mapped to real Hub labels and one left unmapped.](../_embeds/convert-legacy-tk-labels-02.png)

5. Review the preview. It lists every label, notice, and whole-project reference that will change, how many content items each affects, and whether it "Will be reassigned" or "Will be skipped — map this label to include it." Select the "Back to mapping" button to adjust your mapping, or the "Confirm & Run Batch" button to proceed. This button is hidden if no content will be affected.

    ![The preview step listing each label with its affected node count and outcome.](../_embeds/convert-legacy-tk-labels-03.png)

6. Wait for the batch to finish. A message reports how many items were updated, and names any labels or notices that were left unmapped so you can address them later.

    ![A status message reporting nodes updated, and a warning naming a label left unmapped.](../_embeds/convert-legacy-tk-labels-04.png)

## Remove content from an unmappable label

Some legacy labels or notices may have no real equivalent on the Hub. To fully retire a legacy project, remove these from content directly instead of mapping them.

1. On the Manage Projects page, a legacy project that still has content attached shows an "Active — referenced by *N* node(s)" status. Select this link.

    ![The legacy projects table showing an "Active — referenced by" link for a project with remaining content.](../_embeds/convert-legacy-tk-labels-05.png)

2. On the resulting page, find the label or notice you want to remove, then select its "Review & remove" link.

    ![A legacy project's breakdown page listing a label still referenced by content, with a Review & remove link.](../_embeds/convert-legacy-tk-labels-06.png)

3. Select the content items you want to remove the label or notice from. Items are unchecked by default, so only what you check is affected.

    ![The review page with a checkbox table of content referencing the label, a few items checked.](../_embeds/convert-legacy-tk-labels-07.png)

4. Select the "Continue to Confirm" button.
5. Review the list of selected items, then select the "Remove" button to permanently remove the label or notice from them. Other labels, notices, and projects on those items aren't affected.

    ![The confirmation page listing selected content items and a warning that the removal cannot be undone.](../_embeds/convert-legacy-tk-labels-08.png)

    Once the label has been removed from every item referencing it, the breakdown page confirms there's nothing left to address.

    ![The breakdown page after removal, reading "No individual labels or notices are still referenced."](../_embeds/convert-legacy-tk-labels-09.png)

## Decommission a legacy project

Once a legacy project has no remaining content references, whether because everything was reassigned or removed, you can decommission it to permanently delete its cached legacy label and notice data.

1. On the Manage Projects page, confirm the legacy project's status reads "Active — no remaining references."

    ![The legacy projects table comparing a project still referenced by content to one with no remaining references.](../_embeds/convert-legacy-tk-labels-10.png)

2. Select the checkbox next to the project.

    ![The legacy projects table with a project's checkbox selected.](../_embeds/convert-legacy-tk-labels-11.png)

3. From the dropdown menu, select "Decommission," then select "Apply action."

    ![The "With selected items" dropdown set to Decommission next to the Apply action button.](../_embeds/convert-legacy-tk-labels-12.png)

4. Review the confirmation page, then select the "Decommission" button. This cannot be undone.

    ![The Decommission confirmation page listing the selected legacy project and a permanent-deletion warning.](../_embeds/convert-legacy-tk-labels-13.png)

    The project no longer appears in the legacy projects table once it's decommissioned.

    ![The legacy projects table after decommissioning, with only one legacy project remaining.](../_embeds/convert-legacy-tk-labels-14.png)

## Related articles

- [Understanding Legacy Traditional Knowledge Labels](UnderstandingLegacyTKLabels.md)
- [Manage Local Contexts Projects](ManageLocalContextsProjects.md)
