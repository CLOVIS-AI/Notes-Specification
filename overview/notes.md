# Overview: notes

Notes are the primary entity of the project.

A note is composed of:
- a title,
- a description,
- a list of elements.

Elements are composed of:
- a description,
- a flag marking whether they are ticked.

[TOC]

## Creating notes

Users may create a note by providing a title and description.
When creating a note, the creator is given full rights.

## Access rights

Notes can be shared with other users.
In the following list, roles are listed in ascending order of access rights; that is, each role has all the rights of all roles listed before itself.

- Limited read-only: users can see the title, the description, and un-ticked elements.
- Read-only: users see ticked elements.
- Contributor: users can add elements, un-tick elements and remove elements, see the list of other accounts having access to the note.
- Full rights: users can share and un-share the note with other users, archive or unarchive the note, delete the note, edit the title and description.

## Listing notes

Users can list all notes they have access to.

## Modification history

The history remembers all modification made to a note, including its archival status, changes to its title and description, which elements were ticked or un-ticked and by whom, etc.
Each history event should store:
- The account who did the action,
- The time at which the action was made,
- The action that was taken.

Users can see history events if they are allowed to see their consequences. For example:
- Users below Contributor cannot see the list of users having access to the note, so they cannot see who did actions if it is not themselves,
- Limited read-only users cannot see ticked elements, so they cannot see ticking and un-ticking events. However, they can see changes to the title and description,
- Contributors cannot see archival status events,
- Users with full rights can see all events.
