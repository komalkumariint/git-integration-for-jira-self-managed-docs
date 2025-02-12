---

title: Branches API
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

The Branches REST API will obtain list of branches associated to a Jira issue.

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        There are two types of users who can perform the Branches API call:
        <ol>
            <li>Jira <b>administrators</b></li>
            <li>Jira user who has <b>all</b> of the following:
            <ol type='a'>
                <li><b>View/browse permissions</b> to the project;</li>
                <li><b>View Development Tools permissions</b> to the same project; and</li>
                <li>The repository is <b>associated</b> to the project.</li>
            </ol>
            </li>
        </ol>
    </div>
    </div>
</div>
<br>

## Branches

### url
`/rest/gitplugin/1.0/issues/branches?`**key**`=`**{issuekey}**

### method
GET

### Parameters

| Parameter | Description |
| :--- | :--- |
| _**issueKey**_ | _String_. Optional.<br><br>This is the Jira Issue Key – a concatenation of Project key and Issue number. It must contain a dash ('-'). The _**issueKey**_ must be valid and existent.<br><br>For example: `TST-435`. |

### Response

If the _optional query_ is not defined, it will return all indexed git branches.

### Example

`http://jira.yourorg.com/rest/gitplugin/1.0/issues/branches?`**key="TST-435"**

```json
Result:
{
    "success":true,
    "branches":["master","release","TST-435"]
}
```

<br>
<br>
<hr>
<br>
<br>

**[« Back to REST API index](/git-integration-for-jira-data-center/rest-api-gij-self-managed)**

