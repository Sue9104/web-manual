# Glossary

<!-- toc -->

## Visibility level

|Level|Description|
| :--- | :--- |
|private|This project is only visible for project members (owner, translator, reviewer, and guest). |
|public|This project is visible for every logged-in user. |


## Entry status

<span id='entry-status'></span>

An entry has five states: unassigned, untranslated, unretranslated, unreviewed and qualified.
Therefore, the sum of entry counts with five status equals to total counts of project entries.

$$ Total = $$
$$ \sum unassigned + \sum untranslated + \sum unretranslated + \sum unreviewed + \sum qualified $$

![](/assets/entry_status.png)

<table>
  <tr>
    <th>Entry Status</th>
    <th>Dashboard</th>
    <th>Workspace</th>
    <th>Worker</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>unassigned</td>
    <td>Assignment</td>
    <td>Project Management &gt; <b>Assignment</b></td>
    <td>Owner</td>
    <td>Entry has not been assigned to translator.</td>
  </tr>
  <tr>
    <td>untranslated</td>
    <td rowspan="2">Translation</td>
    <td>Translation Management &gt; <b>Translation</b></td>
    <td rowspan="2">Translator</td>
    <td>Entry is assigned to you and has not been translated.</td>
  </tr>
  <tr>
    <td>unretranslated</td>
    <td>Translation Management &gt; <b>Retranslation</b></td>
    <td>Entry's latest translation is rejected by reviewer and has not been retranslated.</td>
  </tr>
  <tr>
    <td>unreviewed</td>
    <td>Review</td>
    <td>Review Management &gt; <b>Review</b> </td>
    <td>Reviewer</td>
    <td>Entry is translated and has not been reviewed. </td>
  </tr>
  <tr>
    <td>qualified</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>Entry has been well translated and the translation can't be modified before version release.</td>
  </tr>
</table>

## Issue status

<span id='issue-status'></span>

If one project member opened an issue about entry's wrong translation, the owner need to recheck the translation and reply it as soon as possible.

![](/assets/issue_status.png)

Once the issue was agreed, the translation status changed to "Error".

<table>
  <tr>
    <th>Issue Status</th>
    <th>Dashboard</th>
    <th>Workspace</th>
    <th>Worker</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>unresolved</td>
    <td>Issues</td>
    <td rowspan="3">Released Projects &gt; <b>Issues</b> </td>
    <td rowspan="3">Owner</td>
    <td>Owner has not replied to the issue yet.</td>
  </tr>
  <tr>
    <td>agreed</td>
    <td rowspan="2">-</td>
    <td>Owner agreed with the issue and revived the translation.</td>
  </tr>
  <tr>
    <td>ignored</td>
    <td>Owner disagreed with the issue and ignored it.</td>
  </tr>
</table>

## Translation status

Once the entry's translation is finished, it will go through two stages: review and released correction.
<span id='translation-status'></span>

![](/assets/translation_status.png)

| Translation Status | Description |
| :--- | :--- |
| Unreviewed | This translation has not been reviewed. |
| Passed | This translation passed the review. |
| Failed | This translation did not pass the review. |
| Error | This translation was released in a version, but some project members thought it was wrong and the owner agreed. |

