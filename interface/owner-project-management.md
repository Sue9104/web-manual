# Owner: Project Management

- [Overview](#overview)
  - [Project Detail](#detail)
    - [Setting](#setting)
    - [Schedule](#schedule)
    - [Upload](#upload)
    - [Release](#release)
- [Assignment](#assign)


## Overview

<span id='overview'></span>


The projects created by you are listed here. "Total" is the total counts of project entries, and "Completed" is the percentage of entries with qualified translation. 

- If you want to know more information about one project, _**Double click**_ the row or click "Detail".

- If you want to add new project, click "New Project".

- If the project is highlighted in pink, it means the project has not finished before the deadline.

![](/assets/project_management.overview.png)

### Project Detail
<span id='detail'></span>

User can easily manage a project from four aspects: "Setting", "Schedule", "Upload" and "Release".

#### Setting
<span id='setting'></span>

Setting shows the configuration when you created the project.

- All settings are editable except owner and creation date. Furthermore, visibility level is only allowed to change from private to public. 

- Delete the project is only allowed when nothing has been uploaded.

- If more people want to join in, click **Add Member > Edit**. It is forbidden to delete member for record traceability now.

![](/assets/project_management.setting.png)

#### Schedule
<span id='schedule'></span>

Schedule is divided into two categories: project schedule and member schedule.

- Project schedule summaries the progress of project stages (assignment, translation and review).

- Member schedule calculates the complete percentage of each project member. 

![](/assets/project_management.schedule.png)

> Only owner is in charge of assignment, so owner's task equals to total counts of project entries (10).
>
> Since translation review is not assigned, so the total reviewers' task equals to total counts of **translated entries** (5\*80% + 2\*100% = 6).

Furthermore, there is a shortcut for owner's task: translation assignment ("Assignment") and issue resolvement ("Issues").

#### Upload

<span id='upload'></span>

"Upload File" is the only way to add or append database entries in Trantrace. It has a specific requirement for the file.

1. Support file types:
  - comma-delimited (.csv) or tab-delimited (.tsv) text file.
  - Single-page spreadsheet (.xls or .xlsx) from Microsoft Excel.
2. File name:
  - Only support  letters (A-Za-z), numbers (0-9), dot (.), hypen (-), and underscore (\_).
  - Make sure the extension is correct.
3. File size:
  - 10MB or less.
4. Content:
  - The first row must be the header.
  - The first column must be unique.

![](/assets/project_management.upload.png)

#### Release
<span id='release'></span>

A new version is published with version id by clicking "New Version". Moreover, all historical versions are listed below.

![](/assets/project_management.release.png)

## Assignment

<span id='assign'></span>

Assignment is the first step of task-based translation cooperation. Owner should assign entries to translator once the database file was uploaded.

> Please see [entry status](../glossary.md#entry-status) for description of status.

![](/assets/project_management.assignment.png)

**Operations:**

1. **Assign one entry to one translator**: fill in translator and click "Assign".

2. **Assign multiple entries to one translator**: select entries in current page or "Search" results, then click "Batch Allocation".

3. **Search entries by project name, keyword and status**
