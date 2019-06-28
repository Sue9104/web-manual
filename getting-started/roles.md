# Role

## User role 

<span id='system-roles'></span>

There are two roles in Trantrace: root and regular user.

| Role | Permission | Workspace |
| :--- | :--- | :--- |
| root | add new user and reset user password | [Root Interface](../interface/root.md) |
| regular user | create projects and others (assign, translate, review and search) depending on the role in project | [User Interface](../interface/user.md) |

## Project role

Each user in Trantrace shares same interface but has different workspace. There are four roles in one project: owner, translator, reviewer and guest.

| Role | Permission | Workspace |
| :--- | :--- | :--- |
| owner | change settings, upload files, assign entries to translator and release versions | [Project Management](../interface/owner-project-management.md) |
| translator | **translate** assigned entries from owner and **retranslate** failed entries from reviewer | [Translation Management](../interface/translator-translation-management.md) |
| reviewer | decide whether to let the translation pass review based on quality | [Review Management](../interface/reviewer-review-management.md) |
| guest | search translation of released projects and open an issue if the translation is error | [Released Projects](../interface/guest-released-projects.md) |




