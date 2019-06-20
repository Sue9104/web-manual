# Roles

## System roles 

<span id='system-roles'></span>

There are two roles in the Trantrace system: root and user. 

| Role | Permissions | Workspace |
| :--- | :--- | :--- |
| root | add or delete users | [Root Interface](../interface/root.md) |
| user | manage projects and others (assign、translate、review、comment) depending on the role in project | [User Interface](../interface/user.md) |

## Project Roles

Each user in Trantrace shares same interface but has different workspace. There are four roles in one project: owner, translator, reviewer, guest.

| Role | Permissions | Workspace |
| :--- | :--- | :--- |
| owner | change settings, upload files, assign tasks to translators and release versions | [Project Management](../interface/owner-project-management.md) |
| translator | **translate** assigned tasks from owner and **retranslate** failed items from reviewers | [Translation Management](../interface/translator-translation-management.md) |
| reviewer | decide whether to let the translation pass or fail | [Review Management](../interface/reviewer-review-management.md) |
| guest | search the released databases and comment if the translations is error or improper | [Released Projects](../interface/guest-released-projects.md) |




