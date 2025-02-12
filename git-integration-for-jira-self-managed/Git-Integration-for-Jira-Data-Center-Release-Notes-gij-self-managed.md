---

title: Git Integration for Jira Data Center/Server - Release Notes
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

We publish new features, bug fixes, security updates/patches, and Jira compatibility regularly. Below are highlights of the changes.

**Important links**

*   [Roadmap for Git Integration for Jira Server/Data Center](https://trello.com/b/WRrWMs87/git-integration-server-data-center-roadmap)

*   [Atlassian Marketplace listing](https://marketplace.atlassian.com/apps/4984/git-integration-for-jira?hosting=datacenter&tab=overview)

*   [Git Integration for Jira Server/Data Center Security](https://www.gitkraken.com/git-integration-for-jira/security-and-trust)


If you have any questions, please contact us through our [Support Portal](https://help.gitkraken.com/git-integration-for-jira-data-center/gij-self-hosted-contact-support/) or by emailing [gijsupport@gitkraken.com](mailto:gijsupport@gitkraken.com)

* * *

## Dedicated indexing nodes for Jira Data Center

`22 Mar 2022` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b>

New General setting for specifying specific DC nodes to perform Git Integration for Jira indexing jobs.

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/gitdc-gencfg-indexing-allow-all-nodes-specific.png?version=1&modificationDate=1648202939114&cacheVersion=1&api=v2)

## Added support for SSH config file

`14 Mar 2022` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b>

Support for the [SSH Config File](https://linuxize.com/post/using-the-ssh-config-file/) was implemented when connecting repositories via SSH.

## Enforce GitHub permissions to view Git data

`01 Mar 2022` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b>

*   Jira administrators can require Jira users to provide a GitHub personal access token to verify repository permission to view all development information provided by the Git Integration for Jira app.

*   When enabled, GitHub permissions are required to see: Repositories, Commits, Branches, Pull Requests and Tags.

*   Limited to GitHub.com and GitHub Enterprise Server git services. Support for GitLab and Azure DevOps available at a later date.


## Data Center indexing job improvements

`09 Dec 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#FFF1B6; padding:1px 5px; color:#172A4C; border-radius:3px; margin: 0 5px; font-size: small;'>INDEXING</b>

*   Queue shared between all Data Center nodes.

*   Each node has a separate indexing job thread for faster indexing times.


## Repository indexing skipping

`09 Dec 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b>

*   **Skipping** -- Duplicate indexing tasks on the same repositories are not added to the queue.


## Webhook indexing sleep setting

`09 Dec 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b> <b style='background-color:#FFEBE6; padding:1px 5px; color:#C02909; border-radius:3px; margin: 0 5px; font-size: small;'>WEBHOOK SETTING</b>

*   **Sleep** -- Prevents repositories' indexing tasks from being added too often. (5)


![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/image-20211209-031238.png?version=1&modificationDate=1639021594011&cacheVersion=1&api=v2)

## View all repositories renamed to Repository browser

`09 Dec 2021` <b style='background-color:#DEEAFE; padding:1px 5px; color:#0C42A3; border-radius:3px; margin: 0 5px; font-size: small;'>IMPROVEMENT</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

_View all repositories_ has been renamed to _Repository browser_ for consistency.

## ${basebranch} Branch name template

`09 Dec 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b> <b style='background-color:#FFF1B6; padding:1px 5px; color:#172A4C; border-radius:3px; margin: 0 5px; font-size: small;'>GENERAL SETTINGS</b>

We have added the `${basebranch}` variable to the Branch name template in [General settings](/git-integration-for-jira-data-center/general-settings-gij-self-managed).

## Deep Linking to GitKraken

`21 Sep 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

With the [acquisition](https://www.gitkraken.com/blog/gitkraken-acquires-git-integration-jira-bigbrassband) of BigBrassBand's Git Integration for Jira app (GIJ) by GitKraken, we have introduced deep linking between GIJ and GitKraken so users can now have a stronger integration between the two. You can now click to open commits, branches, tags and repositories directly in GitKraken from the Jira issue view giving you a seamless transition from your Jira issues to GitKraken.

[Learn more](https://link.bigbrassband.com/docs-gitserverdc-integration-with-gitkraken)

You will see the added ability to open the GitKraken client from our app in various locations. See an example of what this looks like below.

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/server-screen%20copy.png?version=1&modificationDate=1636580970015&cacheVersion=1&api=v2)

## Native Jira audit logging support

`26 Mar 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#FFF1B6; padding:1px 5px; color:#172A4C; border-radius:3px; margin: 0 5px; font-size: small;'>GENERAL SETTINGS</b>

With the auditing feature, key activities are tracked on the Jira instance. This provides administrators insight on how the instance is being used.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/gencfg-audit-log.png?version=2&modificationDate=1618649456348&cacheVersion=1&api=v2&width=374&height=74)![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/audit-logging.png?version=1&modificationDate=1622578322231&cacheVersion=1&api=v2)

The audit log functionality is also extended to Jira Data Center instances as it will have more coverage areas, various event volume levels and an option to integrate the audit log file with external tools.

For more information on this feature, see [**General settings – Audit log settings**](/git-integration-for-jira-data-center/audit-log-settings-gij-self-managed).

## Automatically add link to Jira issue in PRs/MRs created in a Jira issue

`26 Mar 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b>

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/CleanShot2021-06-01%20at%2015.23.50@2x-20210601-192353.png?version=1&modificationDate=1622578333469&cacheVersion=1&api=v2)

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/image-20210328-071823.png?version=1&modificationDate=1618649456408&cacheVersion=1&api=v2)

Pull/merge requests created via the git integration developer panel in the Jira issue will automatically add a link to the Jira issue where it was created from.

## Add JMESPath support for Gerrit integration

`26 Mar 2021` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b>

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/gitserver-gerrit-jmespath-filter-option.png?version=1&modificationDate=1618649456413&cacheVersion=1&api=v2&width=544&height=357)

Gerrit auto-connect integration now supports JMESPath. This feature is used to filter and limit which repositories are integrated.

## Add JMESPath support for tracked folders

`04 Dec 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Tracked folder integration now supports JMESpath. This feature is used to filter and limit which repositories are integrated. For more information, read about JMESPath expressions on their [website](https://jmespath.org/).

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/jira-serverdc-add-tracked-folder-jmespath-advanced.png?version=1&modificationDate=1611738996438&cacheVersion=1&api=v2&width=442&height=163)

Follow this feature in [**this article**](/git-integration-for-jira-data-center/working-with-jmespath-filters-gij-self-managed).

* * *

## Associate Pull/Merge requests to issues based on commits

`27 Nov 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

A new setting has been added in General Settings that allows for pull request (PR) and merge request (MR) indexing via API. In earlier versions, automatic indexing of PR/MRs could not be avoided for auto-connect integrations. With this implementation, administrators can enable/disable this feature as a setting.

Additionally, the PR/MR will still be linked to the Jira issue even if users didn’t mention a Jira issue key in the PR/MR title or description – as long as it’s mentioned in a commit message.

The following settings are implemented in the **Manage git repositories** page ➜ **General settings** under **Git pull/merge requests**.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/jira-server-general-settings-branch-pull-req-cfgs%20(c).png?version=1&modificationDate=1611742804892&cacheVersion=1&api=v2&width=544&height=362)

For more information, follow [**this article**](/git-integration-for-jira-data-center/associate-pull-merge-requests-to-issues-based-on-commits-gij-self-managed).

* * *

## Add support for new AWS CodeCommit region: Europe (Milan)

`09 Oct 2020` <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Europe (Milan) has been added to the supported region list in the AWS CodeCommit integration.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/jira-serverdc-aws-cc-eu-milan-region-add.png?version=1&modificationDate=1611745484608&cacheVersion=1&api=v2&width=612&height=433)

* * *

## Reimplement pull/merge request indexing

`17 Sep 2020` <b style='background-color:#DEEAFE; padding:1px 5px; color:#0C42A3; border-radius:3px; margin: 0 5px; font-size: small;'>IMPROVEMENT</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

This is an improvement of the feature which requires a full reindex after upgrading the app to switch over to the new PR handling.

* * *

## Introduced cron style scheduling option for some General settings

`17 Sep 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ADMINS</b>

By scheduling jobs in [**Git Integration for Jira**](https://marketplace.atlassian.com/4984) for Server and Data Center (in the **General settings** page) Jira administrators gain control over when jobs run.

![Scheduled jobs showing repository indexing and gc](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/general-settings-scheduled-jobs.png?version=1&modificationDate=1611748710415&cacheVersion=1&api=v2&width=544&height=217)

For detailed information, see [**this article**](/git-integration-for-jira-data-center/scheduling-jobs-gij-self-managed),

* * *

## Deduplicate webhook indexing triggers

`17 Sep 2020` <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

This is an optimization feature where the new reindex request is skipped whenever there's a similar occurrence in the queue. This process does not involve repositories that are currently being indexed.

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>DATA CENTER</b> This implementation requires cluster lock usage to enforce synchronization between threads (webhook, manual, and scheduled reindex) and between nodes.
    </div>
    </div>
</div>
<br>

* * *

## Automatically import repos from Gerrit

`19 May 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Gerrit integration has been added to the Auto-connect integration panel. Access this feature via the dashboard menu **Git** ➜ **Manage repositories**.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/jira-serverdc-new-autoconnect-ui.png?version=1&modificationDate=1611822418749&cacheVersion=1&api=v2&width=612&height=174)

Follow this feature in the [**Gerrit integration guide**](/git-integration-for-jira-data-center/gerrit-gij-self-managed).

* * *

## Extend Commits API to show branch name

`19 May 2020` <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

The Commits REST API has been extended to show branch name in the results.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/jira-serverdc-branches-commits-api-example.png?version=1&modificationDate=1611825301037&cacheVersion=1&api=v2&width=442&height=468)

For more information, see [**Commits REST API**](/git-integration-for-jira-data-center/commits-api-gij-self-managed).

* * *

## Branch and PR/MR creation improvements

`19 May 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b> <b style='background-color:#DEEAFE; padding:1px 5px; color:#0C42A3; border-radius:3px; margin: 0 5px; font-size: small;'>IMPROVEMENT</b>

**Branch creation**

*   Improved message matching in how Jira displays it.

*   Added clickable link to respective git hosts in the message which opens in a new tab/window.

    ![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/jira-serverdc-branch-add-msg.png?version=1&modificationDate=1611833546033&cacheVersion=1&api=v2)

<br>

**Branch deletion**

*   Improved message matching in how Jira displays it.
 
    ![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/jira-serverdc-branch-del-msg.png?version=1&modificationDate=1611833572873&cacheVersion=1&api=v2)

<br>

**Pull/merge request creation**

*   Automatically selects the first branch that has the Jira issue key in the branch title from the **Source branch** list.

*   Improved message matching in how Jira displays it.

    ![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/jira-serverdc-autosel-branch-from-list-first-one-if-many.png?version=1&modificationDate=1611842239570&cacheVersion=1&api=v2) |

For related information, see [**Creating Pull/Merge Request**](/git-integration-for-jira-data-center/creating-branches-and-pull-merge-requests-basics-gij-self-managed).

* * *

## Support for Azure Files as storage for Jira Data Center

`03 Mar 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Git Integration for Jira app **VERSION 3.5+** now supports Azure Files as storage for Jira Data Center.

* * *

## Support Azure DevOps/VSTS/TFS webhooks

`03 Mar 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Git Integration for Jira app **VERSION 3.5+** now supports webhooks for Azure DevOps/VSTS/TFS instances.

For more information, read [**Adding Webhooks for Azure DevOps/VSTS**](/git-integration-for-jira-data-center/adding-webhooks-for-azure-devops-repos-vsts-gij-self-managed) and [**Adding Webhooks for Azure DevOps Server/TFS**](/git-integration-for-jira-data-center/adding-webhooks-for-azure-devops-server-tfs-gij-self-managed) in Confluence.

* * *

## REST API to manage integrations

`03 Mar 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

The REST APIs for the following articles were updated with refspec support:

*   Integration ([Add New Integration](/git-integration-for-jira-data-center/add-new-integration-gij-self-managed), [Update Existing Integration](/git-integration-for-jira-data-center/update-existing-integration-gij-self-managed)

*   Repository ([Add New Repository](/git-integration-for-jira-data-center/add-new-repository-gij-self-managed), [Update Existing Repository](/git-integration-for-jira-data-center/update-existing-repository-gij-self-managed)

*   Bulk Change ([Bulk Export](/git-integration-for-jira-data-center/bulk-export-gij-self-managed), [Bulk Import](/git-integration-for-jira-data-center/bulk-import-gij-self-managed)


See also **Fetch Refspec** with Auto-Connect Integration wizard in _**Advanced**_ options:

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/image-20210130-065758.png?version=1&modificationDate=1611989883536&cacheVersion=1&api=v2&width=510&height=179)

<br>

The refspec options are available for supported auto-connect integrations via the Git Integration configuration page:

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/image-20210130-070135.png?version=1&modificationDate=1611990100009&cacheVersion=1&api=v2&width=510&height=122)

* * *

## Added support for new AWS CodeCommit region: Asia Pacific (Hong Kong)

`03 Mar 2020` <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Asia Pacific (Hong Kong) has been added to the supported region list in the AWS CodeCommit integration.

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/jira-serverdc-aws-cc-asiapacific-region-add.png?version=1&modificationDate=1611990576907&cacheVersion=1&api=v2)

* * *

## New Smart Commit command: Label

`03 Mar 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

The new smart commit **\#label** adds a new label to a Jira issue. The label(s) are added to all mentioned Jira issues where more than one Jira issue key is referenced. Several labels can be created by introducing spaces between words for each label.

**Syntax:**

**ISSUE\_KEY #label \[label1\] .. \[labelN\]**

| Example 1 | Example 2 |
| :--- | :--- |
| `ABC-123` **#label** `bucketbreakfix` `bucketenhancement` | ABC-123 #label this-is-a-label |
| **Result** | **Result** |
| Creates four (4) labels `bucketbreakfix` and `bucketenhancement` to the **ABC-123** Jira issue. | Creates the label `this-is-a-label` to the **ABC-123** Jira issue. |

<br>

| Screens for Example 1 |
| :---: |
| ![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/image-20210201-090037.png?version=1&modificationDate=1612170042752&cacheVersion=1&api=v2&width=442&height=201) |
| ![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/image-20210201-090111.png?version=1&modificationDate=1612170076399&cacheVersion=1&api=v2&width=442&height=155) |

* * *

## Show last three and first tag in sidebar

`03 Mar 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

The Git Integration for Jira app will show the last three and first tags if no filter is set. If the filter is set, the Git for Jira app will use it and will display the tags sorted in ascending order by date.

If there are several git tags listed, click the **more...** label link to expand the list in increments of five tags.

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1078231449/image-20210201-090855.png?version=1&modificationDate=1612170538758&cacheVersion=1&api=v2)

* * *

## Add safeguard to Smart Commits processing

`07 Feb 2020` <b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px; font-size: small;'>NEW FEATURE</b> <b style='background-color:#EAE5FE; padding:1px 5px; color:#412C92; border-radius:3px; margin: 0 5px; font-size: small;'>ALL USERS</b>

Adds **Max. commit age** setting to General Settings which:

*   Sets a limit (in days) for Smart Commit processing.

*   Commits older than the Max commit age can be associated with the Jira issue but any Smart Commit commands will not be processed.

*   Protects against cases where old commits are merged into a new repository.


![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1078231449/image-20210201-091335.png?version=1&modificationDate=1612170818610&cacheVersion=1&api=v2&width=340&height=74)

