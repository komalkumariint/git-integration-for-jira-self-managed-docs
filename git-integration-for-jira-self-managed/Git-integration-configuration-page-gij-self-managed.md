---

title: Git integration configuration page
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

![](/wp-content/uploads/gij-gitserver-manage-git-repo-screen.png)

<br>

On this page, you will be able to setup your git repositories and connect them to Jira via Manage git repositories page. Utilize the following features for git integration and configuration:

- [Add new integration panel](#add-new-integration-panel)
- [Connect to Git repository](#connect-to-git-repository)
- [Enable all or Disable all](#enable-all-or-disable-all)
- [Bulk change](#bulk-change)
- [Indexing options](#indexing-options)
- [Webhooks](#webhooks)
- [Related helpful tips](#related-helpful-tips)

<br>
<hr>
<br>

## Add new integration panel

![](/wp-content/uploads/gij-gitserver-git-manager-add-new-integration-panel.png)

Formerly known as Auto-Connect integration panel.

In here, you will find special integration options for specific git hosts. This feature supports multiple connected repositories and automates git integration.

<div class="bbb-callout bbb--tip">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        We highly recommend this feature for multiple repository configuration.
    </div>
    </div>
</div>

For more details on supported git hosts, see the Auto-connect section in our [Integration guides](/git-integration-for-jira-data-center/integration-guides-gij-self-managed).

The **Add tracked folder** connection feature is added to the **Add new integration** panel for easy access.

<div class="bbb-callout bbb--error">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>GitLab</b><br>
        We are dropping support for Gitlab API v3. Please use <b>GitLab API v4</b> when adding new integrations for increased security.
    </div>
    </div>
</div>
<br>

## Connect to Git repository

![](/wp-content/uploads/gij-gitserver-connect-git-repo.png)

This feature opens the Connect wizard.

You can connect single git repositories using this setup such as git protocol, SSH, HTTP/HTTPS, etc. Clicking the adjacent **…** will open the dropdown list of integration options such as [Add tracked folder](/git-integration-for-jira-data-cemter/tracked-folders-gij-self-managed) and equivalent integration connection options. |

## Enable all or Disable all

![](/wp-content/uploads/gij-gitserver-enable-disable-all.png)

The **Enable all** function will enable each integration in the repository list and mark all checkboxes in the _**Enabled**_ column.

The **Disable all** function will disable each integration in the repository list and unmark all the checkboxes in the _**Enabled**_ column.

## Bulk change

![](/wp-content/uploads/gij-gitserver-bulk-change.png)

Bulk change provides an easier way to import or export repository configuration. This feature is useful when you are migrating from an old server to a new server and is also recommended when upgrading to a new version of Git Integration for Jira app.

**Export Configuration** &nbsp;&ndash;&nbsp; this function will export your repository integration configuration to a tab-delimited file (.TSV).

**Import Configuration** &nbsp;&ndash;&nbsp; this function will import your repository integration configuration from a tab-delimited file (.TSV).

For more information, see [Bulk change](/git-integration-for-jira-data-center/bulk-change-gij-self-managed).

## Indexing options

![](/wp-content/uploads/gij-gitserver-reindex-reset-index-all.png)

**Reindex all integrations** &nbsp;&ndash;&nbsp; this function will perform a reindex queue of all integrations in the repository list. Disabled integrations are ignored.

<b style='background-color:#E2FCEF; padding:1px 5px; color:#006745; border-radius:3px; margin: 0 5px 0 0; font-size: small;'>NEW FEATURE &mdash; VERSION 4.7+</b><br> **Reset all indexes** &nbsp;&ndash;&nbsp; Jira administrator can start the reset index process for all repositories using "Reset all" in the "Indexing" dropdown menu on the "Manage Git Integrations for Jira" page.

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        Indexing operations may require several hours for large and/or numerous repositories.
    </div>
    </div>
</div>
<br>

For more information on this topic, see [Reindexing](/git-integration-for-jira-data-center/reindexing-gij-self-managed).

## Webhooks

![](/wp-content/uploads/gij-gitserver-webhooks-sidebar.png)

Opens the Webhooks configuration page. Enable/disable webhooks to trigger immediate reindex of the connected git repositories and integration.

For more information about this topic, click [here](/git-integration-for-jira-data-center/integration-webhooks-gij-self-managed) to go to the **Webhooks documentation page**.

## Related helpful tips

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>SSH</b><br>
        When setting up repositories with the Git Integration app, you need to have the necessary access permissions on the private key on the Git server to proceed.
    </div>
    </div>
</div>

<div class="bbb-callout bbb--note">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Windows Server</b><br>
        For cases when git repositories are hosted at Windows servers (Windows Server network drive) — while it is using the Windows server networking, the network credentials accessing the git repository must be the same as the user running Jira.
    </div>
    </div>
</div>

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Windows Network Share</b><br>
        When using Windows network sharing for the repository origin, it is recommended to allocate repositories’ paths shorter than 256 characters.
        <p>Example: <code>\\WS129\custom-repo\project-z\</code></p>
        <p style='margin-bottom: 0 !important'>Otherwise, the provided URL will not be recognized as valid.</p>
    </div>
    </div>
</div>

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>For Jira hosted on Windows</b><br>
        When using Active Directory accounts for repository access, changing the password of the AD account running Jira can cause repository authentication issues.
        <p style='margin-bottom: 0 !important'>The solution for this is to restart Jira to regain access to repositories.</p>
    </div>
    </div>
</div>

<div class="bbb-callout bbb--info">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Repository REST API</b><br>
        As of <b>v2.8.3+</b> of the Git Integration for Jira app, the REST API for managing repositories are implemented. The documentation for this feature is available at <a href='/git-integration-for-jira-data-center/repository-api-gij-self-managed'>Repository REST API</a>.
    </div>
    </div>
</div>

<div class="bbb-callout bbb--info">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Integration REST API<b><br>
        As of <b>v3.5.0.2+</b> of the Git Integration for Jira app, the REST API for managing integrations are implemented. The documentation for this feature is available at <a href='/git-integration-for-jira-data-center/integration-api-gij-self-managed'>Integration REST API</a>.
    </div>
    </div>
</div>
<br>

<br>
<br>

[**Prev:** Setting up repositories](/git-integration-for-jira-data-center/setting-up-repositories-gij-self-managed)

[**Next:** Using the Add new integration wizard](/git-integration-for-jira-data-center/using-the-add-new-integration-wizard-gij-self-managed)


