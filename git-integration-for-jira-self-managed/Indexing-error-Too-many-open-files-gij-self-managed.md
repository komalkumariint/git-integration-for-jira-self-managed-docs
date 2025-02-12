---

title: Indexing error - Too many open files
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

## Problem

Repository is not indexing and errors in Jira logs point to "Too many open files".

## Diagnosis

Jira admins will see a message similar to the one below in the Jira `/application-logs/atlassian-jira.log`:

**Error**

```java
2019-05-07 15:41:13,171 bigbrassband-gitplugin-RevisionIndexerImpl:thread - 0 ERROR      [c.b.j.g.s.indexer.revisions.RevisionIndexerImpl] Unable to index repository 'name' (repoId: 111)
org.eclipse.jgit.errors.TransportException: Failure updating tracking ref refs/...: Too many open files
	at org.eclipse.jgit.transport.FetchProcess.executeImp(FetchProcess.java:229)
	at org.eclipse.jgit.transport.FetchProcess.execute(FetchProcess.java:124)
	at org.eclipse.jgit.transport.Transport.fetch(Transport.java:1271)
	at com.bigbrassband.jira.git.services.gitmanager.SingleGitManagerImpl.fetch(SingleGitManagerImpl.java:1249)
	at com.bigbrassband.jira.git.services.indexer.revisions.GitPluginIndexManagerImpl.fetchImpl(GitPluginIndexManagerImpl.java:510)
	at com.bigbrassband.jira.git.services.indexer.revisions.GitPluginIndexManagerImpl.callFetch(GitPluginIndexManagerImpl.java:497)
	at com.bigbrassband.jira.git.services.indexer.revisions.GitPluginIndexManagerImpl.updateIndex(GitPluginIndexManagerImpl.java:335)
	at com.bigbrassband.jira.git.services.indexer.revisions.RevisionIndexerImpl$1.doRun(RevisionIndexerImpl.java:151)
	at com.bigbrassband.jira.git.services.indexer.revisions.QueueEntry.run(QueueEntry.java:82)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)
Caused by: java.io.IOException: Too many open files
	at java.io.UnixFileSystem.createFileExclusively(Native Method)
	at java.io.File.createNewFile(File.java:1012)
	at org.eclipse.jgit.util.FS_POSIX.createNewFileAtomic(FS_POSIX.java:446)
	at org.eclipse.jgit.internal.storage.file.LockFile.lock(LockFile.java:164)
	at org.eclipse.jgit.internal.storage.file.PackedBatchRefUpdate.lockLooseRefs(PackedBatchRefUpdate.java:349)
	at org.eclipse.jgit.lib.BatchRefUpdate.execute(BatchRefUpdate.java:635)
	at org.eclipse.jgit.transport.FetchProcess.executeImp(FetchProcess.java:224)
	... 13 more
```

## Solution

See Atlassian help article about [increasing the number of file handles available to Jira](https://confluence.atlassian.com/jirakb/loss-of-functionality-due-to-too-many-open-files-errors-156862102.html)

<br>

<div class="bbb-callout bbb--info">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Contact Us</b><br>
        If you still have a question - reach out to our <a href='https://help.gitkraken.com/git-integration-for-jira-data-center/gij-self-hosted-contact-support/'>Support Desk</a> or email us at <a href='gijsupport@gitkraken.com'>gijsupport@gitkraken.com</a>.
    </div>
    </div>
</div>
<br>

<p>&nbsp;</p>

## More articles about troubleshooting, workarounds and solutions

[Why I am getting the error, “git-upload-pack not permitted”?](/git-integration-for-jira-data-center/why-i-am-getting-the-error-git-upload-pack-not-permitted-gij-self-managed/)

[Avoid OutOfMemory exceptions by configuring or memory allocation with Jira to accommodate large repositories](/git-integration-for-jira-data-center/avoid-outofmemory-exceptions-by-configuring-or-memory-allocation-with-jira-to-accommodate-large-repositories-gij-self-managed)

[Cannot auto-deploy some tracked repositories: Specified origin is incorrect or not supported](/git-integration-for-jira-data-center/Cannot-auto-deploy-some-tracked-repositories-gij-self-managed)

[Connection Reset when Accessing the Database](/git-integration-for-jira-data-center/Connection-reset-when-accessing-the-database-gij-self-managed)

["Dangerous use of multiple connections" error on local database](/git-integration-for-jira-data-center/Dangerous-use-of-multiple-connections-error-on-local-database-gij-self-managed)

[Duplicate entry 0 for key PRIMARY exceptions in log](/git-integration-for-jira-data-center/Duplicate-entry-0-for-key-PRIMARY-exceptions-in-log-gij-self-managed)

[Error while reindexing – Java heap space / Object too large, rejecting the pack](/git-integration-for-jira-data-center/Error-while-reindexing-Java-heap-space-Object-too-large,-rejecting-the-pack-gij-self-managed)

[Gitolite integration: Why the Git integration app not see the master branch?](/git-integration-for-jira-data-center/Gitolite-integration--why-the-Git-integration-app-not-see-the-master-branch-gij-self-managed)

[Health Check: Database Collation](/git-integration-for-jira-data-center/Health-check--database-collation-gij-self-managed)

**Indexing error – Too many open files** (this page)

[Installation fails when installing manually](/git-integration-for-jira-data-center/Installation-fails-when-installing-manually-gij-self-managed)

[Jira index error: IndexNotFoundException: no segments* file found](/git-integration-for-jira-data-center/Jira-index-error--IndexNotFoundException--no-segments-file-found)

[Malformed input or input contains unmappable characters](/git-integration-for-jira-data-center/Malformed-input-or-input-contains-unmappable-characters-gij-self-managed)

[Personal access token failing Azure DevOps integration with Not Authorized error](/git-integration-for-jira-data-center/Personal-access-token-failing-azure-devops-integration-with-Not-Authorized-error-gij-self-managed)

[Problems with shared home on Azure Storage](/git-integration-for-jira-data-center/Problems-with-shared-home-on-azure-storage-gij-self-managed)

[Pull request index error: org.json.JSONException](/git-integration-for-jira-data-center/Pull-request-index-error--JSONException-gij-self-managed)

[Repositories missing from Azure DevOps integration](/git-integration-for-jira-data-center/Repositories-missing-from-azure-devops-integration-gij-self-managed)

["Service proxy has been destroyed" exceptions in log](/git-integration-for-jira-data-center/service-proxy-has-been-destroyed-exceptions-in-log-gij-self-managed)

[SQLException 'Incorrect string value' in merge requests](/git-integration-for-jira-data-center/sqlexception-incorrect-string-value-in-merge-requests-gij-self-managed)

[SSH key file format is invalid](/git-integration-for-jira-data-center/ssh-key-file-format-is-invalid-gij-self-managed)

[TFS - Not authorized exception when Jira works thru proxy](/git-integration-for-jira-data-center/tfs-not-authorized-exception-when-jira-works-thru-proxy-gij-self-managed)

[Unexpected exception parsing XML document from URL error in log](/git-integration-for-jira-data-center/Unexpected-exception-parsing-XML-document-from-URL-error-in-log-gij-self-managed)

[Why don't I see the Create Branch or Pull Request features?](/git-integration-for-jira-data-center/why-dont-i-see-the-create-branch-or-pull-request-features-gij-self-managed)

<br>
<br>

