---
currentMenu: permissions
---

# Permissions

BoomCMS uses a role based permissions system with user groups.

A role represents a particular action that can be performed within the CMS.
Examples of roles are accessing the asset manager, editing a page, or managing CMS users.

Roles are assigned to groups which can either allow or disallow a role.
A user will then have the roles from all the groups to which they belong merged to determine whether or not they can perform a particular CMS action.

In order to perform a role a user must be a member of at least one group which is allowed to perform a role.
However, if they're also a member of a group to which the role has been denied then this will take precedence and the user will not be able to perform the role.

## Page permissions

Page permissions work along the same lines.
However, in addition to roles being merged across groups they are also inherited down the page tree.
Therefore if a group is given the 'add page' role to the top level page in the site then they will be able to add pages anywhere in the page tree.
If a group is denied a role then the members of that group will not be able to perform the role in that section of the page tree.

Precedence for page permissions is determined by proximity in the page tree where the role is set.