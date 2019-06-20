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

Task summary table, including workload, complete percentage and unfinished counts, is  divided into four parts by task categories (assignment, translation, review, issues). Click on blue unfinished numbers in the last column and it will jump to these unfinished items.

![](/assets/dashboard.png)

Description of table:

||Worker|total|completed|undone|corresponding undone status in MyTask|
|--|--|
|assignment|owner|total item counts|assigned item percentage|unassigned item counts|unassigned|
|translation|translator|counts of items assigned to you| translated percentage |untranslated and retranslated item counts|untranslated & retranslated|
|review|reviewer| translated items | reviewed percentage| unreviewed item counts|unreviewed|
|feedback|owner|counts of items suggested by guests| replied percentage| suggested item counts|suggested|

**Since the review of each entry is not assigned, all reviewers share same progress**.


## MyTask

<span id='mytask'></span>

My task real-time display all undone job into five categories: **'unassigned'** and **'suggested'** for master, **'untranslated'** and **'re-translated'** for translator, **'unreviewed'** for reviewer. Click and it will jump to corresponding workspace. More detail see [status](../glossary.md#status).

![](/assets/mytask.png)
















