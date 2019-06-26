# User Interface

All users share same interface, but have different workspace depending on the role in project. The user interface is comprised of three parts:

- [Dashboard](#stat)
- Workspace for diffent roles
  - [Owner: Project Management](owner-project-management.md)
  - [Translator: Translation Management](translator-translation-management.md)
  - [Reviewer: Review Management](reviewer-review-management.md)
  - [Guest: Released Projects](guest-released-projects.md)
- [MyTask](#mytask)   

![](/assets/interface.user.png)             
                    
## Dashboard

<span id='stat'></span>

Dashboard summaries user's workload, complete percentage and unfinished counts in four panel by categories (assignment, translation, review and issues). Click on blue text in last column and it will jump to unfinished tasks.

![](/assets/dashboard.png)

Description of summary table:

||Worker|Total|Completed|Not Finished|corresponding status in MyTask|
|--|--|
|Assignment|owner|total number of project entries |percentage of assigned entries|counts of unassigned entries|Unassigned|
|Translation|translator|counts of entries assigned to you| percentage of translated entries | counts of untranslated entries from owner and unretranslated entries from reviewer|Untranslated & Unretranslated|
|Review|reviewer| counts of all translated entries | percentage of reviewed entries | counts of unreviewed entries |Unreviewed|
|Issues|owner|counts of issues opened by guest| percentage of replied issues| counts of unreplied issues|Unreplied|

**Since translation review is not assigned, all reviewers share same number in Total, which equal to counts of all translated entries, but have different complete percentage ( counts of entries reviewed by you divide counts of all translatd entries) **.


## MyTask

<span id='mytask'></span>

My task summaries unfinished tasks and updates every minute. These unfinished tasks are divided into five categories: 

- **'Unassigned'** and **'Unreplied'** for owner
- **'Untranslated'** and **'Unretranslated'** for translator
- **'Unreviewed'** for reviewer. 

Click and it will jump to these unfinished tasks. More detail see [status](../glossary.md).

![](/assets/mytask.png)
















