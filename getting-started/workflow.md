# Workflow
 
![](/assets/workflow.png)

Step 1. [**creation:** user (_owner_) creates a project, uploads file and assigns entries' translation to translator.](#create)

Step 2. [**translation:** _translator_ continuously translates until approved by reviewer.](#translate)

Step 3. [**review:** _reviewer_ reviews translation.](#review)

Step 4. [**release:** _all members_ cooperate to optimize translations until all are in good quality.](#iteration)
 
## Step 1. Creation: user (_owner_) creates project, uploads file and assigns entries' translation to translator

<span id='create'></span>

**Owner** initiates the project:

- Create a project: specify a source and target languages, deadline, priority, visibility and description, and designate project members (translator, reviewer, and guest).

- Upload database files: only support comma-delimited (.csv) or tab-delimited (.tsv) text file and single-page spreadsheet (.xls or .xlsx) from Microsoft Excel.

- Assign entries to translator.

![](/assets/step1_creation.png)


## Step 2. Translation: translator continuously translates until approved by reviewer

<span id='translate'></span>

Translator need continuous translation until approved by reviewer:

- Translate assigned entries from owner.

![](/assets/translation_management.translation.png)

- Retranslate failed entries from reviewer.

![](/assets/translation_management.retranslation.png)


## Step 3. Review: reviewer reviews translation

<span id='review'></span>

Reviewer checks translation one by one and decides whether to let it pass or fail.

![](/assets/step3_review.png)


## Step 4. Release: all members cooperate to optimize translations until all are in good quality.

<span id='iteration'></span>

### Release version

Owner releases version according to progress.

![](/assets/step4_release.png)

### Version iteration

- Scenarios

  - **Wrong translation**: one project member opens an issue to point out the error of released translations.

    ![](/assets/open_issue.png)

  - **More entries**: owner uploads a new file to the project.

    ![](/assets/upload.png)

- Procedures

  1. Owner assigns entries to translator. 
    - **Wrong translation**: owner agrees on the issue and reassigns entry's translation to translator;
    ![](/assets/project_management.reply.png)
    - **More entries**: owner assigns the translation of new entries to translator (repeat step1).
    ![](/assets/project_management.assignment.png)
  2. Translator continuously translates until approved by reviewer (repeat step2)
  3. Review reviews translation (repeat step3).
  4. Owner releases version.











