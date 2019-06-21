# Owner: Project Management

- [Overview](#overview)
  - [Detail](#detail)
    - [Setting](#setting)
    - [schedule](#schedule)
    - [upload](#upload)
    - [release](#release)
- [Assignment](#assign)
- [Feedback](#feedback)


## Overview

<span id='overview'></span>


The projects you created are displayed here. If you want to know more information about one project, _**Double click**_ the row of your interested project, and it will jump to the detail.

![](/assets/project_management.overview.png)

### Detail
<span id='detail'></span>

#### Setting
<span id='setting'></span>

All settings are here, and you can edit them except creation date. However, visibility level is only allowed to change from private to public. You can easily adjust the deadline according to project schedule. If more people want to join in, you can add them in "Add Member" panel.

![](/assets/project_management.overview.information.png)
      
#### Schedule
<span id='schedule'></span>

The schedule is divided into two categories: project shedule and member schedule. Project schedule summaries the progress of project stages (assignment, translation and review), and member schedule calculates the complete percentage of each project member. 

Project Schedule:

|Stage|Percentage|
|--|--|
|Assignment| counts\_of\_assigned_entries / total\_number\_of\_project_entries |
|Translation | counts\_of\_translated\_entries / total\_number\_of\_project_entries |
|Review| counts\_of\_entries\_passed\_review / total\_number\_of\_project_entries |

Member Schedule:

|Role| Percentage |
|--|--|
|Owner | counts\_of\_assigned_entries / total\_number\_of\_project_entries |
| Translator | counts\_of\_entries\_translated\_by\_you / ( counts_of_entries_assigned_to_you + counts_of_your_entries_failed_review ) |
| Reviewer | counts\_of\_entries\_reviewed\_by\_you / counts\_of\_all\_translated\_entries |



 "Assginment" and "Feedback" button are two quick way to workspace of assignment and feedback of current project.

![](/assets/project_management.schedule.png)



#### Upload
<span id='upload'></span>

Just click the "Upload" button to add or append items. Current support format is csv (comma-delimited) and click "Download Template" if you don't know the format.

![](/assets/project_management.upload.png)

#### Release
<span id='release'></span>

Just click the "Export New Version" button, and a new version is released. Moreover, all histroical versions are showed.

![](/assets/project_management.release.png)

## Assignment

<span id='assign'></span>

Assignment is the first step of translation process. Owner should allocate items to translators after project creation.

> Description of status please see [status](../glossary.md#status)

![](/assets/project_management.assignment.png)

**Operation:**
1. allocate one item to one translator
2. allocate multiple items to one translator
3. search items by project name, priority, deadline, keyword, status
 
## Feedback

<span id='feedback'></span>

Owner need quickly reply to the suggestion submited by guests. All the suggestion are presented here.

> Description of status please see [status](../glossary.md#status)

![](/assets/project_management.feedback.png)

**Actions:**
1. ignore suggestion
2. accept suggestion and re-assign to one translator

