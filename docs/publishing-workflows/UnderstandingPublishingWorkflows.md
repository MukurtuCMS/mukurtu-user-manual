---
tags:
    - publishing workflows
    - content
---

# Understanding Publishing Workflows

!!! Roles "User roles" 
    Mukurtu manager, Protocol steward, Language steward, Contributor, Curator, Language contributor

## Default content workflow

This is the default workflow that ships at install.

### Publication states

There are three states:

- Draft
- Published
- Archived

### Transitions

There are four possible transitions between those states:

| From                          | To        | Transition name   | User              |
--------------------------------|-----------|-------------------|--------------------
| Draft, Published	            | Draft     | Save as Draft     | Author, Steward   |
| Draft, Published, Archived	| Published | Publish           | Author, Steward   |
| Published	                    | Archived  | Archive           | Mukurtu manager   |
| Archived	                    | Draft     | Restore to Draft  | Mukurtu manager   |

### Who can do what

- Someone who can edit content (the author or protocol/language steward) can `Save as Draft` and `Publish`.
- Mukurtu managers who can view content can `Archive` and `Restore to Draft`.
- Administrators can bypass all permissions and use all transitions on all content.

### Content page operations

- Per-row: all transitions currently valid for that specific content and viewer (not a fixed list).
- Bulk: `Restore to Draft`, `Publish`, `Archive`.

----------

## Editorial workflow

This is a more complex workflow that can be enabled by a Mukurtu manager. It is designed to support a more formal editorial process, where content is reviewed before publication.

### There are five states

- Draft
- Awaiting Review
- Edits Needed
- Published
- Archived

### Transitions

There are eight possible transitions between those states:

| From                                                      | To               | Transition name    | User                    |
------------------------------------------------------------|------------------|--------------------|--------------------------
| Draft, Awaiting Review, Edits Needed, Published	        | Draft            | Save as Draft      | Author, Steward         |
| Draft, Awaiting Review	                                | Awaiting Review  | Submit for Review  | Author, Steward         |
| Awaiting Review, Published	                            | Edits Needed     | Needs Edits        | Steward                 |
| Edits Needed	                                            | Awaiting Review  | Resubmit for Review| Author, Steward         |
| Draft, Awaiting Review, Edits Needed, Published, Archived | Published        | Publish            | Steward                 |
| Published	                                                | Archived         | Archive            | Steward, Mukurtu Manager|
| Archived	                                                | Draft            | Restore to Draft   | Steward, Mukurtu Manager|
| Published, Archived	                                    | Awaiting Review  | Return to Review   | Steward                 |

### Who can do what

- Content authors can `Save as Draft`, `Submit for Review`, and `Resubmit for Review`.
- Protocol Stewards and Language Stewards can perform every transition: `Save as Draft`, `Submit for Review`, `Needs Edits`, `Resubmit for Review`, `Publish`, `Archive`, `Restore to Draft`, and `Return to Review`.
- Mukurtu managers who can view content can `Archive` and `Restore to Draft`.
- Administrators can bypass all permissions and use all transitions on all content.

### Content page operations

- Per-row: all transitions currently valid for that specific content and viewer (not a fixed list).
- Bulk: `Restore to Draft`, `Publish`, `Archive` (for consistency across both workflows). Note that the Editorial-only states `Submit for Review`, `Needs Edits`, `Resubmit for Review`, and `Return to Review` are not exposed as bulk actions.