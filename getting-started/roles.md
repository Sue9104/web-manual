# Role

## User role 

<span id='system-roles'></span>

There are two roles in Trantrace: root and regular user.

| Role | Permission | Workspace |
| :--- | :--- | :--- |
| root | add new user and reset user password | [Administration Interface](../interface/root.md) |
| regular user | create project and others (assign, translate, review and search) depending on the role in project | [User Interface](../interface/user.md) |

## Project role

Each user shares same interface but has different workspace. There are four roles in one project: owner, translator, reviewer and guest (optional).

| Role | Permission | Workspace |
| :--- | :--- | :--- |
| owner | specify setting, upload file, assign entries to translator, release version and reply issue | [Project Management](../interface/owner-project-management.md) |
| translator | **translate** assigned entries from owner and **retranslate** failed entries from reviewer | [Translation Management](../interface/translator-translation-management.md) |
| reviewer | decide whether to let the translation pass review or not | [Review Management](../interface/reviewer-review-management.md) |
| guest | search translation of released projects and open an issue if the translation is error | [Released Projects](../interface/guest-released-projects.md) |

User case diagram:

![](/assets/usercase.png)


