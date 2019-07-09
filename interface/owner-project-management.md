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


The projects created by you are here. "Total" is the total counts of project entries, and "Completed" is the percentage of entries with qualified translation. 

- If you want to know more information about one project, _**Double click**_ the row or click "Detail".

- If you want to add new project, click "New Project".

![](/assets/project_management.overview.png)

### Detail
<span id='detail'></span>

User can easily manage a project from four aspects: "Setting", "Schedule", "Upload" and "Release".

#### Setting
<span id='setting'></span>

Setting shows configurations when you create the project.

- All settings are editable except owner and creation date. Furthermore, visibility level is only allowed to change from private to public. 

- If more people want to join in, click **Add Member > Edit**. It is forbidden to delete member for record traceability now.

![](/assets/project_management.setting.png)

#### Schedule
<span id='schedule'></span>

Schedule is divided into two categories: project shedule and member schedule.

- Project schedule summaries the progress of project stages (assignment, translation and review).

- Member schedule calculates the complete percentage of each project member. 

Project Schedule:

|Stage|Percentage|
|--|--|
|Assignment| counts\_of\_assigned_entries / total\_counts\_of\_project_entries |
|Translation | counts\_of\_translated\_entries / total\_counts\_of\_project_entries |
|Review| counts\_of\_entries\_with\_qualified\_translation / total\_counts\_of\_project_entries |

Member Schedule:

|Role| Percentage |
|--|--|
|Owner | counts\_of\_assigned_entries / total\_counts\_of\_project_entries |
| Translator | counts\_of\_entries\_with\_qualified\_translation / counts_of_entries_assigned_to_you  |
| Reviewer | counts\_of\_entries\_with\_qualified\_translation\_reviewed\_by\_you / counts\_of\_all\_translated\_entries |


![](/assets/project_management.schedule.png)

Furthermore, there is a shortcut for owner's task: translation assignment ("Assignment") and issue reply ("Reply").

#### Upload

<span id='upload'></span>

Click "Upload File" to add or append entries. 

> **[warning] Only support tab-delimited or comma-delimited text file.**
>
> Click "Download Template" if you don't know the format.

![](/assets/project_management.upload.png)

#### Release
<span id='release'></span>

A new version is published with version id by clicking "New Version". Moreover, all histroical versions are listed below.

![](/assets/project_management.release.png)

## Assignment

<span id='assign'></span>

Assignment is the first step of translation cooperation in Trantrace. Owner should assign entries to translator once the project is created.

> Please see [entry status](../glossary.md#entry-status) for description of status.

![](/assets/project_management.assignment.png)

**Operations:**

1. **Assign one entry to one translator**: fill in translator and click "Assign".

2. **Assign multiple entries to one translator**: select entries in current page or "Search" results, then click "Batch Allocation".

3. **Search entries by project name, keyword and status**
 
## Reply

<span id='feedback'></span>

Owner need quick reply to guest's issues.

> Please see [issue status](../glossary.md#issue-status) for description of status.

![](/assets/project_management.reply.png)

**Operations:**

- **Agree on issue and revive entry's translation**: click "Agree"

- **Disagree on issue and translation is good enough**: click "Ignore"
