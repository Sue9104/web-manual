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
| Error | - | - | Entry's translation is error \(Guest suspected the accuary and owner agreed on that\). |



Issue status:

Once guest opened an issue when he found entry's translation is wrong, owner need to recheck the translation and reply it as soon as possible.

| Status | Menu | Dashboard | Worker | Description |
| :--- | :--- | :--- | :--- | :--- |
| Unreplied | Reply & Issues | Issues | Owner | Owner has not replied the issue yet. |
| Agreed | Reply & Issues | - | - | Owner agreed with guest and revive the translation. |
| Error | Reply & Issues | - | - | Owner disagreed with guest  |



