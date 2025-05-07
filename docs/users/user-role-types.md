---
tags:
    - user roles
---

# User Role Types

There are two types of user roles in Mukurtu CMS: site-wide, and group user roles. Roles are not mutually exclusive. Some users may have both types of roles. Roles can change over time as the site grows and responsibilities shift.

Site wide user roles are managed by the Mukurtu administrator and affect the entire site. Things like color scheme, front page styling, taxonomies and collections are managed through site wide user roles. 

Group user roles are managed independently within each group by the community manager or protocol steward. Access to content is managed through the communities and protocols.

### Site-wide roles

#### Administrator
This role is automatically assigned to the account that was created when first setting up a new site. Site administrators have full access to Drupal options (the platform upon which Mukurtu is built). As such, unless the administrator is comfortable with Drupal, we recommend immediately creating a new Mukurtu Administrator account as soon as a new site is configured. Day to day activities should be handled from this account.

#### Mukurtu administrator
Mukurtu administrators handle most of the site-wide management. They create and manage user accounts, review and approve user account requests, assign site-wide roles, create and delete communities, assign community manager roles, manage taxonomies, and have access to roundtrip tools for import and export. 

#### Authenticated user
Authenticated users are registered users. They have a username and a password and can be assigned both site-wide and group user roles. Users that have not been assigned to a role can view public pages, browse pages, and community pages. Digital heritage items and dictionary words under open protocols are also visible. Users can also create their own personal collections out of existing content.

#### Anonymous User
Anonymous users are non-registered users who are simply browsing the site. They can view public pages and content, but cannot be assigned a user role.

## Group Roles

### Community roles

#### Community manager
Community managers are assigned by the Mukurtu administrator and are responsible for managing membership in the community. They can create and manage new user accounts and review and approve account requests. They can also add and remove users from communities, create new cultural protocols, review and approve or deny subscription requests and manage Local Contexts projects and directories.

When a Mukurtu adminstrator creates a new community, they are automatically assigned to the community manager and protocol steward roles of the new community and protocol. These roles can be assigned to other users, who can then remove the Mukurtu administrator, subjecting them to the requirements of the community and cultural protocols just like any other user.

Community managers are also responsible for the look and feel of the community page. This includes the title, banner and thumbnail images, description, featured content and other display settings.

#### Community member
Community members have basic membership in the community.  If they have not been added to any protocols, they can view the community page and any public content.

From this role, the community manager may assign them other roles and protocols within the community.

#### Community affiliate
This role is designated for users who aren't part of the community but work with the community in some capacity that requires a level of access to community content. Some examples include researchers, archivists and other collaborative partners. Community affiliates may be assigned other roles and protocols within the community.

### Cultural protocol roles

#### Protocol steward
Protocol stewards are assigned by the community manager. They can add and remove protocol members and assign and remove member, affiliate, contributor and steward roles.

Protocol stewards have full permission to create, edit and delete digital heritage items, community records, and multi-page documents and media under their protocol.
	
Protocols stewards also manage the look and feel of the protocol page, including managing the title, banner and thumbnail images, description, protocol type and other advanced display settings. 

#### Protocol member
Protocol members can view the protocol page and any content within the protocol. They can also view comments left on content within the protocol. There is one exception: When content under multiple protocols requires membership in all protocols to access this content, the user will need to meet those requirements to view the item. To learn more about sharing settings for multi-protocol content, see [Understanding Sharing Settings](../3Cs/UnderstandingSharingSettings.md)

#### Protocol affiliate
The protocol affiliates role serves the same purpose as  community affiliates. The role identifies protocol members that are not part of the real-life community but are still allowed access to content within a given protocol. For consistency, when adding community affiliates to a protocol, you may want to assign them a protocol affiliate role.

#### Contributor
Contributors have the same privileges and responsibilities as protocol members. They can also create and edit their own digital heritage items, person records, dictionary words and media assets, and apply protocols to content and media.

#### Community record steward
Community record stewards have the same privileges and responsibilities as protocol members. Additionally, they can edit their own community records and media assets. They can also apply protocol to content and media.

#### Curator
Curators have the same privileges and responsibilities as protocol members, and can create and manage collections and apply protocols to content and media.

#### Language steward
In Mukurtu 4, languages are managed within cultural protocols. There are no separate language communities. 

Language stewards have the same privileges and responsibilities as protocol members. Additionally, they can create and manage all dictionary words and word lists within the protocol and apply protocols to content and media.

#### Language contributor
Language contributors have the same privileges and responsibilities as protocol members and can also create and manage their own dictionary words and word lists within the protocol.

#### Non-member
Non-members can view public material.

To read more about managing membership in communities and protocols, see [Manage Community Membership and Roles](ADD LINK)
