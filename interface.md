# Interface

> The interface varies from [system roles](roles.md#system-roles) in Trantrace. Root has a unique panel user management, and users all share same interface.

+ [root interface](#root)
+ [user interface](#user) 
 - [personal statistics](#stat)
 - [Workspace for different roles](#workspace)
   - [Master: project management](#master)
   - [Translator: translate management](#translator)
   - [Reviewer: review management](#reviewer)
   - [Guest: Released database](#guest)

## Root Interface

<span id='root'></span>

Only root has the permission to add and delete users. Noteably, the record will still exist even if the user has been disabled.

![](/assets/interface.root.png)

### Actions

1. Search exised user by email: click 'Search' button 

2. Add new user: click the "+ New User" button

3. Enable/Disable user: User can login to Trantrace with this button on, otherwise user can not login but their records and operations are still reservered.
 
4. Reset password: this button will reset user password to "123456".


## User Interface

<span id='user'></span>

All users share same interface, but have different workspace depending on the role in project.
 
### Personal Statistics

<span id='stat'></span>

All the workload and complete percentage will be listed by project:
- **allocation**: if you are master of one project, the total item numbers, allocated and unallocated percentage will show here.
- **conflict handling**: if you are master of one project, suggestion numbers, processed and unprocessed will show here.
- **translation**: if you are translator of one project, the item numbers that assigned to you, translated and unretranslated percentage will show here.
- **review**: if you are reviewer of one project, the item numbers that have been translated, reviewed and unreviewed percentage will show here. **Since the reviewers have not been allocated by master, all reviewers share same progress**.

### Workspace for Different Project Role

<span id='workspace'></span>

#### Master: Project Management

<span id='master'></span>

1. 
Click 'detail' button for more information.

- **Settings**: All the settings can be adjusted according to the progress, such as project name, deadline, priority level, visibility level, source and target languages. 

   Actions:

  - **add more project members**: master can easily add a new member from the select. 
  
    

- **Progress Track**

Master can assign task to translator 

- **Import Files**

Just click the "Upload" button to add or append items. Current support format is csv (comma-delimited) and tsv (tab-delimited).

- **Version Control**

Just click the "Export" button, and a new version is released. Moreover, all histroical versions are listed below the button.

#### Translator: Translation Management

<span id='translator'></span>


herwrs 


#### Review: Review Management

<span id='reviewer'></span>


#### Guest: Released Search
<span id='guest'></span>




