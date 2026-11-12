---
tags:
    - publication tools
    - submission forms
    - content
---

# Understanding Submission Forms

!!! roles "User roles" 
    Mukurtu manager

Mukurtu has the ability to provide submission forms for users and visitors to submit content for review and inclusion in the site. A submission form for each Mukurtu content type is provided.

## Configuring notifications

To access submission form settings, from the **Dashboard** select **Submission Forms** or go directly to`/admin/config/mukurtu/submissions`

All Administrators and Mukurtu managers will receive an email notification when a submission form is submitted. To notify other users, you can add them to the **Additional reviewers to notify** list by searching for their username. You can also email other users by adding them to the **Additional reviewers to email** list, though they will still need to log in to the site with appropriate permissions to view the submissions.

Select **Save configuration** when done.

## Enabling and configuring submission forms

By default, submission forms are disabled. To enable submission forms, from the **Dashboard** select **Submission Forms** or go directly to`/admin/config/mukurtu/submissions`

A submission form is provided for each content type. To enable a submission form for a content type, select **Edit**.

From here you can change the name of the submission form, enable and disable the form, select who can submit forms, include introduction and thank you messages, and select which fields and media types are included in the form.

### Label

This is displayed at the top of the submission form. The default is "Submit a [content type]".

### Enable and disable

Enable and disable the submission form for this content type with the "Enable the submission form for this content type" toggle.

### Who can submit?

There are two settings available for who can submit content through the submission form:

- **Visitors and authenticated users** - anyone can submit content through the submission form, including visitors with no user account. This allows public submissions.
- **Authenticated users** - only users who are logged in to the site can submit content through the submission form. This allows users to submit content through a simpler workflow than the standard contributor permissions.

### Submission information

Enable and disable the "Ask submitters how they expect this item to be shared" text field. Since submitted content does not include communities and protocols, information provided here may help that decision during review.

### Introductory text

This is shown on the form before the fields. You can use this to provide instructions or other information to users submitting content.

### Thank-you message

This is shown after the form is submitted. You can use this to provide instructions or other information to users after they submit content. If left blank, a generic message is shown instead.

### Fields and groups

By default, all of the fields in the content type are included in the submission form. They also follow the same tab grouping as the regular content creation forms. 

You can enable and disable fields and groups to customize the submission form so that it is tailored to your needs. For example, if you only want to include a small number of fields for a more streamlined submission form, you can disable the other fields and groups. You can also change the order of the fields and groups by dragging and dropping them into the desired order.

### Allow media types

You can select which media types are allowed to be submitted through the submission form. By default, all media types are allowed. For example if you don't want to allow upload of potentially large video files, or potentially risky iframe embeds, those can be disallowed.

## Links to submission forms

Once a submission form is enabled, a link to the form is provided on the **Submission Forms** page. You can copy this link and share or embed it where needed.