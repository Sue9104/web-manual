# Role

## User role 

<span id='system-roles'></span>

There are two roles in Trantrace: administrator and general user.

<table>
  <tr>
    <th>Role</th>
    <th>Permission</th>
    <th>Workspace</th>
  </tr>
  <tr>
    <td>administrator</td>
    <td>
      <li>Add new user without registration.</li>
      <li>Activate or deactivate user account.</li>
      <li>Reset user password to 123456.</li>
    </td>
    <td><a href="../interface/root.md">Administration Interface</a></td>
  </tr>
  <tr>
    <td>general user</td>
    <td>
      <li>Creat own projects.</li>
      <li>Others depending on the role in project.</li>
    </td>
    <td><a href="../interface/user.md">User Interface</a></td>
  </tr>
</table>

## Project role

General users all share the same interface but have different workspace depending on the project role. There are four roles in one project: owner, translator, reviewer and guest (optional).

Once the project visibility is set to public, every logged in user is the project guest and they all can search released translation and open issues.

<table>
  <tr>
    <th>Role</th>
    <th>Permission</th>
    <th>Workspace</th>
  </tr>
  <tr>
    <td rowspan="2">owner</td>
    <td>
      <li><b>Specify setting</b>, including deadline, priority, source and target language, visibility and members.</li> 
      <li><b>Upload the database files</b> to be translated and large file should be splited to multiple small files.</li>
      <li><b>Assign entries</b> to translator.</li>
      <li><b>Release version</b> for qualified translation.</li>
    </td>
    <td><a href="../interface/owner-project-management.md">Project Management</a></td>
  </tr>
  <tr>
    <td>
      <li><b>Search released translations</b> from joined project.</li>
      <li><b>Resolve issues.</b></li>
    </td>
    <td><a href="../interface/all-released-projects.md">Released Projects</a></td>
  </tr>
  <tr>
    <td rowspan="2">translator</td>
    <td>
      <li><b>Translate assigned entries</b> from owner.</li>
      <li><b>Retranslate failed entries</b> from reviewer.</li>
    </td>
    <td><a href="../interface/translator-translation-management.md">Translation Management</a></td>
  </tr>
  <tr>
    <td>
      <li><b>Search released translations</b> from joined project.</li>
      <li><b>Open issues if found error.</b></li>
    <td><a href="../interface/all-released-projects.md">Released Projects</a></td>
  </tr>
  <tr>
    <td rowspan="2">reviewer</td>
    <td><li><b>Review translation</b> to decide whether to let it pass or not.</li></td>
    <td><a href="../interface/reviewer-review-management.md">Review Management</a></td>
  </tr>
  <tr>
    <td>
      <li><b>Search released translations</b> from joined project.</li>
      <li><b>Open issues if found error.</b></li>
    </td>
    <td><a href="../interface/all-released-projects.md">Released Projects</a></td>
  </tr>
  <tr>
    <td>guest</td>
    <td>
      <li><b>Search released translations</b> from joined project.</li>
      <li><b>Open issues if found error.</b></li>
    </td>
    <td><a href="../interface/all-released-projects.md">Released Projects</a></td>
  </tr>
</table>

User case diagram:

![](/assets/usercase.png)


