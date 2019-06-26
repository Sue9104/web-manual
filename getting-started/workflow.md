# Workflow
 
![](/assets/Trantrace_workflow.jpg)

Step 1. [**creation:** user (_owner_) create project, upload files and assign entries' translation to translator](#create)

Step 2. [**translation:** _translator_ continously translates until approved by reviewer](#translate)

Step 3. [**review:** _reviewer_ reviews translation ](#review)

Step 4. [**version iteration:** _all members_ cooperate to optimize translations until all are in good quality](#iteration)
 
## Step 1. Creation: user (_owner_) creates project, uploads files and assigns entries' translation to translator

<span id='create'></span>

**Owner** initiates the project:

- Create a project: specifies source and target languages, deadline, priority, visibility and description, and designate project members (translator, reviewer and guest)

- Upload database **csv** files: only support csv file and max filesize 10Mb.

- Assign translation of entries to translators

![](/assets/step1_creation.png)

## Step 2. Translation: translator continously translates until approved by reviewer

<span id='translate'></span>

Translator need continous translation until approved by reviewer:

- translate entries assigned by owner.

![](/assets/translation_management.translation.png)

- retranslate entries rejected by reviewer.

![](/assets/translation_management.retranslation.png)


## Step 3. Review: reviewer reviews translation

<span id='review'></span>

Reviewer check translations one by one and decide whether to let it pass or fail.

![](/assets/step3_review.png)

## Step 4. Version Interation: all members cooperate to optimize translations until all are in good quality.

<span id='iteration'></span>

### Release version

Owner releases version according to progress.

![](/assets/step4_release.png)

### Iteration

- Scenarios

  - **wrong translation**: guest opens an issue to point out the error, and owner agrees on that and revives the translation.

    ![](/assets/open_issue.png)

  - **more entries**: owner adds more entries to the project.

    ![](/assets/upload.png)

- procedures

  1. owner assigns job to translator. 
    - **wrong translation**: owner replies guest's issue and reassigns entry's translation to translator;
    ![](/assets/project_management.reply.png)
    - **more entries**: owner assigns the translation of new entries to translator (step1).
    ![](/assets/project_management.assignment.png)
  2. translator contiously translates until approved by reviewer (step2)
  3. review reviews translation (step3).
  4. owner releases version.











