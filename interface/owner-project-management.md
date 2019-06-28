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


The projects you created are here. "Total" is the counts of project entries, and "Completed" is the percentage of entries with qualified translation. 

- If you want to know more information about one project, _**Double click**_ the row or click "Detail".

- If you want to add new project, click "New Project" button.

![](/assets/project_management.overview.png)

### Detail
<span id='detail'></span>

#### Setting
<span id='setting'></span>

All settings are editable except owner and creation date. Furthermore, visibility level is only allowed to change from private to public. 

- If more people want to join in, click "Edit" in "Add Member" panel. It is forbidden to delete member for record traceability now.

![](/assets/project_management.overview.setting.png)
      
#### Schedule
<span id='schedule'></span>

Schedule is divided into two categories: project shedule and member schedule.

- Project schedule summaries the progress of project stages (assignment, translation and review).

- Member schedule calculates the complete percentage of each project member. 

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
| Translator | counts\_of\_entries\_with\_qualified\_translation / counts_of_entries_assigned_to_you  |
| Reviewer | counts\_of\_entries\_reviewed\_by\_you / counts\_of\_all\_translated\_entries |


![](/assets/project_management.schedule.png)

Furthermore, there is a shortcut for owner's task: translation assignment ("Assignment") and issue reply ("Reply").

#### Upload

<span id='upload'></span>

Click "Upload File" to add or append entries. Current support format is csv, which is delimted by comma (,) and enclosed by quote ("). Click "Download Template" if you don't know the format.

![](/assets/project_management.upload.png)

#### Release
<span id='release'></span>

A new version is published with version id by clicking "Release New Version". Moreover, all histroical versions are listed below.

![](/assets/project_management.release.png)

## Assignment

<span id='assign'></span>

Assignment is the first step of the translation process. Owner should assign entries to translator after creation.

> Description of status please see [entry status](../glossary.md#entry-status)

![](/assets/project_management.assignment.png)

**Operations:**

1. Assign one entry to one translator: fill in translator and click "Assign".

2. Assign multiple entries to one translator: select entries in current page or "Search" results, click "Batch Allocate".

3. Search entries by project name, keyword and status
 
## Reply

<span id='feedback'></span>

Owner need quick reply to guest's issues.

> Description of status please see [issue status](../glossary.md#issue-status)

![](/assets/project_management.reply.png)

**Operations:**

- Revive translation: click "Agree"

- Do not retranslation: click "Ignore"
