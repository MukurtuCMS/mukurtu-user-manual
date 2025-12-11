---
tags:
- users
- account management
---
# Manage User Accounts from a Site-wide Role

!!! Roles "User roles" 
    Administrator, Mukurtu manager

## Manage individual user accounts
Once a user account has been created, you can return to that user's form and edit their account information. To do this, select the **people** icon on the left-hand sidebar. 
![Dashboard with sidebar menu and people icon highlighted in red](../_embeds/add-user-account-01.png)

You will see a list of all site users. Find their username, and select the **edit** button in their row. 
![User list with edit button highlighted](../_embeds/add-user-account-12.png)

Make any desired edits and select **Save**. Refer to the [Create a new user account](../users/creating-account-site-wide.md) article for detail on each field.

You will be returned to the user list and a success message will be displayed.
![User list with success message displayed](../_embeds/add-user-account-13.png)

## Bulk manage user accounts
You can also make certain changes to user accounts in bulk. Available changes are:

- Send notifications daily
    - A digest of notifications will be sent on a daily basis.
- Send notifications immediately 
    - Notifications will be sent immediately as they are generated.
- Send notifications weekly 
    - A digest of notifications will be sent on a weekly basis.
- Add the administrator role to the selected users 
    - The selected users will be assigned the administrator role 
- Add the Mukurtu Manager role to the selected users (use with extreme caution!)
    - The select users will be assigned the Mukurtu manager role.
- Block the selected user(s) 
    - The status of the user will be changed from "active" to "blocked"
- Cancel the selected user account(s)
    - Applying this action will open a secondary page where you will select a cancellation method.
- Remove the administrator role from the selected user(s) 
    - The administrator role and associated acceess and capabilities will be removed from the user(s)
- Remove the Mukurtu manager role from the selected user(s) 
    - The Mukurtu manager role and associated access and capabiltiites will be removed from the user(s)
- Unblock the selected user(s) 
    - The user's status will be changed from "blocked" to "active."

1) To use any of these actions on one or more members, from the manage members page, check the box next to each name you wish to manage. 

2) Using the action menu at the bottom of the page, select the action you wish to apply. 

3) Select **Apply to selected items**. The action will be applied to all selected members.
![The people page, with two users selected, and action menu item selected. These, along with the apply button are highlighted](../_embeds/add-user-account-14.png)

4) You will receive different results depending on the action item you select. Below are descriptions of the results of applying steps 1-3 above for each action item, and any additional instructions as needed.

### Send notifications daily 
1. Complete steps 1-3.
![People page with two users selected and the "Send notifications daily" action selected](../_embeds/add-user-account-15.png)

2. A success message is displayed. (Verify this)
SCREENSHOT 16
![People page with success message displayed](../_embeds/placeholderscreenshot.png)

### Send notifications immediately
1. Complete steps 1-3.

![People page with two users selected and the "Send notifications immediately" action selected](../_embeds/add-user-account-17.png)

2. A success message is displayed. (Verify this)
SCREENSHOT 18
![People page with success message displayed](../_embeds/placeholderscreenshot.png)

### Send notifications weekly
1. Complete steps 1-3.
![People page with two users selected and the "Send notifications weekly" action selected](../_embeds/add-user-account-19.png)

2. A success message is displayed. (verify this)
SCREENSHOT 20
![People page with success message displayed](../_embeds/placeholderscreenshot.png)

### Add the administrator role to the selected users
1. Complete steps 1-3.
![The people page with two users selected and the action item "Add the administrator role to the selected users" selected](../_embeds/add-user-account-21.png)

2. A success message is displayed, and the administrator role is applied to the selected users.
![The people page reloaded with a success message. The added administrator role is highlighted](../_embeds/add-user-account-22.png)

### Add the Mukurtu Manager role to the selected users
1. Complete steps 1-3.
![The people page with two users selected and the action item "Add the Mukurtu Manager role to the selected users" is selected](../_embeds/add-user-account-23.png)

2. A success message is displayed, and the Mukurtu manager role is applied to the selected users.
![The people page reloaded with a success message. The added Mukurtu manager role is highlighted](../_embeds/add-user-account-24.png)

### Block the selected user(s)
1. Complete steps 1-3.
![The people page with two users selected and the action item "Block the selected user(s)" is selected](../_embeds/add-user-account-25.png)


2. A success message is displayed, and the selected users are blocked.
![The people page reloaded with a success message. The selected users are blocked. Their status is highlighted.](../_embeds/add-user-account-26.png)

### Cancel the selected user account(s)
There are several cancellation methods that yield different results.

1. Complete steps 1-3, then select one of the cancellation methods on the next page. Below are additional details about each cancellation method.
![The people page with two users selected and the action item Cancel the select user account(s) selected.](../_embeds/add-user-account-27.png)

#### Disable the account and keep its content
Disabling the account and keeping its content will block the user and keep any content they created available on the site.They will be listed as the creator of the content item. You can unblock the user at any time.

2. Select **Disable the account and keep its content.**
![The cancellation methods form with Disable the account and keep its content selected](../_embeds/add-user-account-28.png)

3. Use the toggle to notify the user of the cancellation. This is optional.

4. Select **Confirm**. You will be returned to the people page and a success message will be displayed. The user's status will be set to "blocked."
![The people page with a confirmation message displayed. The users' status is set to blocked.](../_embeds/add-user-account-29.png)

#### Disable the account and unpublish its content
Disabling the account and unpublishing its content will block the user. Any content they created will be unpublished. Administrators can view this content by adding `admin/content` to the end of your web address (i.e. http://mysite.org/admin/content). Note that the content page is inaccessible to Mukurtu managers.

You can unblock the user at any time. If the content is re-published, the user will still be listed as the author of the content items.

2. Select **Disable the account and unpublish its content.**
![The cancellation methods form with Disable the account and unpublish its content selected](../_embeds/add-user-account-30.png)

3. Use the toggle to notify the user of the cancellation. This is optional.

4. Select **Confirm**. You will be returned to the people page and a success message will be displayed. The user's status will be set to "blocked," and any content they created will be unpublished. 
![The people page with a confirmation message displayed. The users status is set to blocked.](../_embeds/add-user-account-31.png)

#### Delete the account and make its content belong to the Anonymous User. 

!!! Warning 
    This cannot be undone

Deleting the account and assigning its content to the Anonymous user will completely delete the user(s). Any content they created will remain available, but will be listed as created by "Anonymous User". Proceed with caution, as this cannot be undone.

1. Select **Delete the account and make its content belong to the Anonymous User.**
![The cancellation methods form with delete the account and make its content belong to the Anonymous User selected.](../_embeds/add-user-account-32.png)

2. Use the toggle to notify the user of the cancellation. This is optional.

3. Select **Confirm**. You will be returned to the people page and a success message will be displayed. The user will be deleted and their account no longer visible or accessible. Any content they created will be assigned to "Anonymous User."
![The people page with a confirmation message displayed. The users is deleted.](../_embeds/add-user-account-33.png)

#### Delete the account and its content
!!! Warning 
    This cannot be undone

Deleting the account and its content will completely delete the user(s) and all associated content. Proceed with caution, as this cannot be undone.

1. Select **Delete the account and its content.**
![The cancellation methods form with Delete the account and its content selected.](../_embeds/add-user-account-34.png)

2. Use the toggle to notify the user of the cancellation. This is optional.

3. Select **Confirm**. You will be returned to the people page and a success message will be displayed. The user will be deleted and their account no longer visible or accessible. Any content they created will also be deleted.
![The people page with a confirmation message displayed. The users is deleted.](../_embeds/add-user-account-35.png)

### Remove the administrator role from the selected user(s) 
1. Complete steps 1-3.
![The people page with two users selected and the action item "Remove the administrator role from the selected user(s)" is selected](../_embeds/add-user-account-36.png)

2. A success message is displayed, and the administrator role is removed from the selected users.
![The people page reloaded with a success message. The selected users are are no longer administrators](../_embeds/add-user-account-37.png)

### Remove the Mukurtu manager role from the selected user(s) 
1. Complete steps 1-3.
![The people page with two users selected and the action item "Remove the Mukurtu manager role from the selected user(s)" is selected](../_embeds/add-user-account-38.png)

2. A success message is displayed, and the Mukurtu manager role is removed from the selected users.
![The people page reloaded with a success message. The selected users are no longer Mukurtu Managers. Their role is highlighted](../_embeds/add-user-account-39.png)

### Unblock the selected user(s)
1. Complete steps 1-3.
![The people page with two users selected and the action item "Unblock the selected user(s)" is selected](../_embeds/add-user-account-40.png)

2. A success message is displayed, and the selected users are now set to active.
![The people page reloaded with a success message. The selected users are set to active. Their status is highlighted.](../_embeds/add-user-account-41.png)
