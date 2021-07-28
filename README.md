# A POC for Group Content Moderation

This is a basic site with a single content type and permission set to try to determine the correct permission set
for group content moderation.

## Role Definitions and Goals

Drupal Roles:
Site Admin: Will have site level "administrative type" permissions to create groups as needed.

Site Editor: Have the same site level permissions as site admin for creating content, but cannot create groups.

Group Types:
Public Content: This is a single group type to allow published content of the group to be viewable to anonymous users,
but editing of the group content is limited to members of the group.

Group:
Prime Group: The only group for this POC.

Group Roles:
Contributor: Should be able to create content, create a new draft, send to review

Reviewer: Should be able to review content and set as "ready to publish," return to draft, or leave at "needs review"

Approver: Should be able to use all moderation transitions

Group Administrator: Same permissions as approver, but can also administer group users

**Problem** All users have access to ALL transitions despite set permissions.

### Testing

A set of test users is created for local development testing.

**User:** site_editor_contributor **Password:** siteeditor

**User:** site_editor_reviewer **Password:** siteeditor

**User:** site_editor_approver **Password:** siteeditor

**User:** site_admin_contributor **Password:** siteadmin

**User:** site_admin_reviewer **Password:** siteadmin

**User:** site_admin_approver **Password:** siteadmin

For admin access to review permissions settings:

**User:** admin **Password:** admin

## Getting Started

You must first have [Docksal installed](https://docs.docksal.io/getting-started/) and setup on your computer.

From your terminal, go to the directory where you have cloned the repo and enter the following command:
```
fin init
```
