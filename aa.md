```
| Status | Before/After version | Description | Worker | Workspace in menu |Dashboard|
```

```
| :--- | :--- | :--- | :--- | :--- |:--- |
| unassigned | before | this item is not assigned | owner | Assignment |Assignment|
| untranslated | before | this item is not translated | translator | Translation |Translation|
| re-transalted | before | translation is refused by reviewer and need another translation | translator | Re-translation |Translation|
| unreviewed | before | translation is not reviewed | reviewer | Review |Review|
| qualified | before | translation is approved | reviewer | Review |Review|
| suggested | after | guest submit a suggestion for translation | owner | Feedback |Feedback|
| error | after | owner accepted guest suggestion, and mark this item wrong | owner | Feedback |Feedback|
```

| Status | Dashboard | Worker | Description |
| :--- | :--- | :--- | :--- |
| Unassigned | Assignment | Owner | Entry is not assigned to translator. |
| Untranslated | Translation | Translator | Entry is assigned to you and needs to be translated. |
| Unretranslated | Translation | Translator | Entry is rejected by reviewer and needs to be retranslated. |
| Unreviewed | Review | Reviewer | Entry is translated and needs to be reviewed. |
| Qualified | - | - | Entry's translation is good enought and can't be modified before version release. |
| Error | - | - | Entry's translation is error \(Guest suspected the accuary and owner agreed and revive the translation\). |

Issue status:

Once guest opened an issue about entry's wrong translation, owner need to recheck the translation and reply it as soon as possible.

| Status | Dashboard | Worker | Description |
| :--- | :--- | :--- | :--- |
| Unreplied | Issues | Owner | Owner has not replied the issue yet. |
| Agreed | - | - | Owner agreed with guest and revived the translation. |
| Ignored | - | - | Owner disagreed with guest and ignored it. |



Translation history and review history:

| Status | Description |
| :--- | :--- |
| Pass | This translation passed the review of reviewer. |
| Fail | This translation did not pass the review of reviewer. |
| Error | This translation is considered to be error by owner and guest. |



