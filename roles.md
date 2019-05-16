# Roles

## System roles <span id='system-roles'></span>

There are two roles in the Trantrace system: root and user.

| Role | Permissions | Workspace |
| :--- | :--- | :--- |
| root | add or delete users | [User Management](interface.md#root) |
| user | build own project, other permissions depending on the role in project | [Project Management](interface.md#user) |

## Project Roles

Each user in Trantrace can build own project and assign different permissions to project members. There are four roles in a specific translation project: master, translator, reviewer, guest.

| Role | Permissions | Workspace |
| :--- | :--- | :--- |
| master | assign task to translators, revise project settings, release version | [Project Management](interface.md#master) |
| translator | translate the assigned items and retranslate the items rejected by reviewers | [Translation Management](interface.md#translator) |
| reviewer | decide whether to accept the translation or not | [Review Management](interface.md#reviewer) |
| guest | search the released database and subnmit suggestions | [Released Database](interface.md#guest) |




