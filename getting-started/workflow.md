# Workflow
 
![](/assets/Trantrace_workflow.png)

Step 1. [**creation:** user (_owner_) creates project, uploads files and assigns entries' translation to translator](#create)

Step 2. [**translation:** _translator_ continously translates until approved by reviewer](#translate)

Step 3. [**review:** _reviewer_ reviews translation ](#review)

Step 4. [**release:** _all members_ cooperate to optimize translations until all are in good quality](#iteration)
 
## Step 1. Creation: user (_owner_) creates project, uploads files and assigns entries' translation to translator

<span id='create'></span>

**Owner** initiates the project:

- Create a project: specify source and target languages, deadline, priority, visibility and description, and designate project members (translator, reviewer and guest).

- Upload database files: only support **csv** file and max filesize 10Mb.

- Assign translation of entries to translators

![](/assets/step1_creation.png)

## Step 2. Translation: translator continously translates until approved by reviewer

<span id='translate'></span>

Translator need continous translation until approved by reviewer:

- Translate entries assigned by owner.

![](/assets/translation_management.translation.png)

- Retranslate entries rejected by reviewer.

![](/assets/translation_management.retranslation.png)


## Step 3. Review: reviewer reviews translation

<span id='review'></span>

Reviewer checks translation one by one and decides whether to let it pass or fail.

![](/assets/step3_review.png)

## Step 4. Relase: all members cooperate to optimize translations until all are in good quality.

<span id='iteration'></span>

### Release version

Owner releases version according to progress.

![](/assets/step4_release.png)

### Iteration

- Scenarios

  - **Wrong translation**: guest opens an issue to point out the error, and owner agrees on that and revives the translation.

    ![](/assets/open_issue.png)

  - **More entries**: owner adds more entries to the project.

    ![](/assets/upload.png)

- Procedures

  1. Owner assigns job to translator. 
    - **Wrong translation**: owner replies guest's issue and reassigns entry's translation to translator;
    ![](/assets/project_management.reply.png)
    - **More entries**: owner assigns the translation of new entries to translator (step1).
    ![](/assets/project_management.assignment.png)
  2. Translator contiously translates until approved by reviewer (step2)
  3. Review reviews translation (step3).
  4. Owner releases version.











