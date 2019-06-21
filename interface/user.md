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

Task summary table, including workload, complete percentage and unfinished counts, is  divided into four parts by task categories (assignment, translation, review, issues). Click on blue unfinished numbers in the last column and it will jump to these unfinished tasks.

![](/assets/dashboard.png)

Description of summary table:

||Worker|Total|Completed|Not Finished|corresponding status in MyTask|
|--|--|
|Assignment|owner|total number of project entries |percentage of assigned entries|counts of unassigned entries|Unassigned|
|Translation|translator|counts of entries assigned by owner and failed by reviewer| percentage of translated entries | counts of untranslated entries from owner and unretranslated item from reviewer|Untranslated & Unretranslated|
|Review|reviewer| counts of all translated entries | percentage of reviewed entries | counts of unreviewed entries |Unreviewed|
|Issues|owner|counts of issues opened by guest| percentage of replied issues| counts of unreplied issues|Unreplied|

**Since translation review is not assigned, all reviewers share same workload but have different actual completed tasks**.


## MyTask

<span id='mytask'></span>

My task summaries unfinished tasks and updates every minute. These unfinished tasks are divide into five categories: **'Unassigned'** and **'Unreplied'** for owner, **'Untranslated'** and **'Unretranslated'** for translator, **'Unreviewed'** for reviewer. Click and it will jump to these unfinished tasks. More detail see [status](../glossary.md#status).

![](/assets/mytask.png)
















