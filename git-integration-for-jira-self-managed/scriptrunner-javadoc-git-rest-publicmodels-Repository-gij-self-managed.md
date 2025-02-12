---

title: ScriptRunner - Javadocs - Class Repository
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

* Package [com.bigbrassband.jira.git.rest.publicmodels](#)
*  *[Object](https://docs.oracle.com/javase/8/docs/api/java/lang/Object.html)*  \> [Repository](#) (this page)

All implemented interfaces :
* *com.bigbrassband.jira.git.services.props.GProperties*




## Summary
#### Constructors

| Visibility | Signature |
| --- | --- |
| `public` | [Repository](#repository)() |
| `public` | [Repository](#repositoryinteger-string)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  id,  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  displayName) |


#### Methods

| Type and modifiers | Method signature |
| --- | --- |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getApiFilter](#getapifilter)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getApiPath](#getapipath)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getAwsRegion](#getawsregion)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getBranchLinkFormat](#getbranchlinkformat)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getChangesetFormat](#getchangesetformat)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getCreateInitialCommit](#getcreateinitialcommit)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getDisplayName](#getdisplayname)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getEnableFetches](#getenablefetches)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getFileAddedFormat](#getfileaddedformat)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getFileDeletedFormat](#getfiledeletedformat)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getFileModifiedFormat](#getfilemodifiedformat)() |
| `public`  *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  | [getFolderDepth](#getfolderdepth)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getGroup](#getgroup)() |
| `public`  *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  | [getId](#getid)() |
| `public`  *[Date](https://docs.oracle.com/javase/8/docs/api/java/util/Date.html)*  | [getInitDate](#getinitdate)() |
| `public` *[IntegrationType](/git-integration-for-jira-data-center/scriptrunner-javadoc-git-services-integration-IntegrationType-gij-self-managed/)* | [getIntegrationType](#getintegrationtype)() |
| `public`  *[Date](https://docs.oracle.com/javase/8/docs/api/java/util/Date.html)*  | [getLastIndexedDate](#getlastindexeddate)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getMainBranch](#getmainbranch)() |
| `public`  *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  | [getMaxMinsToCommitEmail](#getmaxminstocommitemail)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getMergeRequestFormat](#getmergerequestformat)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getOrigin](#getorigin)() |
| `public`  *[Set](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html)* < *[Long](https://docs.oracle.com/javase/8/docs/api/java/lang/Long.html)* > | [getProjectMappingIds](#getprojectmappingids)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getRealRoot](#getrealroot)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getRefSpecCustom](#getrefspeccustom)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getRepositoryHostingUrl](#getrepositoryhostingurl)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getRepositoryKey](#getrepositorykey)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getRevisionIndexing](#getrevisionindexing)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getRoot](#getroot)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getSendCommitEmails](#getsendcommitemails)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getShowAllTags](#getshowalltags)() |
| `public`  *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  | [getSshKeyId](#getsshkeyid)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [getSupportsBranchCreationApi](#getsupportsbranchcreationapi)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getSupportsPullRequestApi](#getsupportspullrequestapi)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getTagsFilter](#gettagsfilter)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getTfsCollection](#gettfscollection)() |
| `public`  *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  | [getTrackedFolderId](#gettrackedfolderid)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getUsername](#getusername)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getViewFormat](#getviewformat)() |
| `public`  *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  | [getWebLinkType](#getweblinktype)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isAbsoluteRoot](#isabsoluteroot)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isCommitsValidationRequired](#iscommitsvalidationrequired)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isDisableSslVerification](#isdisablesslverification)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isDisabled](#isdisabled)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isGitViewerEnabled](#isgitviewerenabled)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isGlobal](#isglobal)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isHosted](#ishosted)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isRefSpecChanges](#isrefspecchanges)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isRefSpecNotes](#isrefspecnotes)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isRequireUserPat](#isrequireuserpat)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isSmartCommitsEnabled](#issmartcommitsenabled)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isSourcesDiffViewEnabled](#issourcesdiffviewenabled)() |
| `public`  *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  | [isTrustFolderStat](#istrustfolderstat)() |
| `public` `void` | [setAbsoluteRoot](#setabsoluterootboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  absoluteRoot) |
| `public` `void` | [setApiFilter](#setapifilterstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  apiFilter) |
| `public` `void` | [setApiPath](#setapipathstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  apiPath) |
| `public` `void` | [setAwsRegion](#setawsregionstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  awsRegion) |
| `public` `void` | [setBranchLinkFormat](#setbranchlinkformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  branchLinkFormat) |
| `public` `void` | [setChangesetFormat](#setchangesetformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  changesetFormat) |
| `public` `void` | [setCommitsValidationRequired](#setcommitsvalidationrequiredboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  commitsValidationRequired) |
| `public` `void` | [setCreateInitialCommit](#setcreateinitialcommitboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  createInitialCommit) |
| `public` `void` | [setDisableSslVerification](#setdisablesslverificationboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  disableSslVerification) |
| `public` `void` | [setDisabled](#setdisabledboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  disabled) |
| `public` `void` | [setDisplayName](#setdisplaynamestring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  displayName) |
| `public` `void` | [setEnableFetches](#setenablefetchesboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  enableFetches) |
| `public` `void` | [setEncryptedPassword](#setencryptedpasswordencryptedstring)(*com.bigbrassband.jira.git.utils.EncryptedString* password) |
| `public` `void` | [setEncryptedPat](#setencryptedpatencryptedstring)(*com.bigbrassband.jira.git.utils.EncryptedString* pat) |
| `public` `void` | [setFileAddedFormat](#setfileaddedformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  fileAddedFormat) |
| `public` `void` | [setFileDeletedFormat](#setfiledeletedformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  fileDeletedFormat) |
| `public` `void` | [setFileModifiedFormat](#setfilemodifiedformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  fileModifiedFormat) |
| `public` `void` | [setFolderDepth](#setfolderdepthinteger)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  folderDepth) |
| `public` `void` | [setGitViewerEnabled](#setgitviewerenabledboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  gitViewerEnabled) |
| `public` `void` | [setGlobal](#setglobalboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  global) |
| `public` `void` | [setGroup](#setgroupstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  group) |
| `public` `void` | [setHosted](#sethostedboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  hosted) |
| `public` `void` | [setId](#setidinteger)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  id) |
| `public` `void` | [setInitDate](#setinitdatedate)( *[Date](https://docs.oracle.com/javase/8/docs/api/java/util/Date.html)*  initDate) |
| `public` `void` | [setIntegrationType](#setintegrationtypeintegrationtype)(*[IntegrationType](/git-integration-for-jira-data-center/scriptrunner-javadoc-git-services-integration-IntegrationType-gij-self-managed/)* integrationType) |
| `public` `void` | [setLastIndexedDate](#setlastindexeddatedate)( *[Date](https://docs.oracle.com/javase/8/docs/api/java/util/Date.html)*  lastIndexedDate) |
| `public` `void` | [setMainBranch](#setmainbranchstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  mainBranch) |
| `public` `void` | [setMaxMinsToCommitEmail](#setmaxminstocommitemailinteger)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  maxMinsToCommitEmail) |
| `public` `void` | [setMergeRequestFormat](#setmergerequestformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  mergeRequestFormat) |
| `public` `void` | [setOrigin](#setoriginstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  origin) |
| `public` `void` | [setPassword](#setpasswordstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  password) |
| `public` `void` | [setPat](#setpatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  pat) |
| `public` `void` | [setProjectMappingIds](#setprojectmappingidsset)( *[Set](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html)* < *[Long](https://docs.oracle.com/javase/8/docs/api/java/lang/Long.html)* > projectMappingIds) |
| `public` `void` | [setRealRoot](#setrealrootstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  realRoot) |
| `public` `void` | [setRefSpecChanges](#setrefspecchangesboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  refSpecChanges) |
| `public` `void` | [setRefSpecCustom](#setrefspeccustomstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  refSpecCustom) |
| `public` `void` | [setRefSpecNotes](#setrefspecnotesboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  refSpecNotes) |
| `public` `void` | [setRepositoryHostingUrl](#setrepositoryhostingurlstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  repositoryHostingUrl) |
| `public` `void` | [setRepositoryKey](#setrepositorykeystring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  repositoryKey) |
| `public` `void` | [setRequireUserPat](#setrequireuserpatboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  requireUserPat) |
| `public` `void` | [setRevisionIndexing](#setrevisionindexingboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  revisionIndexing) |
| `public` `void` | [setRoot](#setrootstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  root) |
| `public` `void` | [setSendCommitEmails](#setsendcommitemailsboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  sendCommitEmails) |
| `public` `void` | [setShowAllTags](#setshowalltagsboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  showAllTags) |
| `public` `void` | [setSmartCommitsEnabled](#setsmartcommitsenabledboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  smartCommitsEnabled) |
| `public` `void` | [setSourcesDiffViewEnabled](#setsourcesdiffviewenabledboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  sourcesDiffViewEnabled) |
| `public` `void` | [setSshKeyId](#setsshkeyidinteger)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  sshKeyId) |
| `public` `void` | [setSupportsBranchCreationApi](#setsupportsbranchcreationapiboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  supportsBranchCreationApi) |
| `public` `void` | [setSupportsPullRequestApi](#setsupportspullrequestapistring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  supportsPullRequestApi) |
| `public` `void` | [setTagsFilter](#settagsfilterstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  tagsFilter) |
| `public` `void` | [setTfsCollection](#settfscollectionstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  tfsCollection) |
| `public` `void` | [setTrackedFolderId](#settrackedfolderidinteger)( *[Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)*  trackedFolderId) |
| `public` `void` | [setTrustFolderStat](#settrustfolderstatboolean)( *[Boolean](https://docs.oracle.com/javase/8/docs/api/java/lang/Boolean.html)*  trustFolderStat) |
| `public` `void` | [setUsername](#setusernamestring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  username) |
| `public` `void` | [setViewFormat](#setviewformatstring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  viewFormat) |
| `public` `void` | [setWebLinkType](#setweblinktypestring)( *[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)*  webLinkType) |
| `public static` *java.util.function.Function*\<*com.bigbrassband.jira.git.services.gitmanager.GitManager*, [Repository](#)\> | [toRepositoryTransformer](#torepositorytransformermultiplegitrepositorymanager)(*com.bigbrassband.jira.git.services.gitmanager.MultipleGitRepositoryManager* repositoryManager) |
| `public static` *java.util.function.Function*\<*com.bigbrassband.jira.git.services.gitmanager.GitManager*, [Repository](#)\> | [toShortFormRepositoryTransformer](#toshortformrepositorytransformermultiplegitrepositorymanager)(*com.bigbrassband.jira.git.services.gitmanager.MultipleGitRepositoryManager* repositoryManager) |



# Constructors
## Repository()




## Repository(Integer, String)




## Repository(GitManager, IntegrationType, boolean)





# Methods
## getApiFilter()
Returns the JMESPath Filter property of the repository.



## getApiPath()
Returns the Custom API Path property of the repository.



## getAwsRegion()
Returns the AWS region property. Used for AWS repositories only.



## getBranchLinkFormat()




## getChangesetFormat()




## getCreateInitialCommit()




## getDisplayName()
Returns the display name of the repository.



## getEnableFetches()




## getFileAddedFormat()




## getFileDeletedFormat()




## getFileModifiedFormat()




## getFolderDepth()




## getGroup()




## getId()




## getInitDate()




## getIntegrationType()




## getLastIndexedDate()




## getMainBranch()




## getMaxMinsToCommitEmail()




## getMergeRequestFormat()




## getOrigin()




## getProjectMappingIds()




## getRealRoot()




## getRefSpecCustom()




## getRepositoryHostingUrl()




## getRepositoryKey()




## getRevisionIndexing()




## getRoot()




## getSendCommitEmails()




## getShowAllTags()




## getSshKeyId()




## getSupportsBranchCreationApi()




## getSupportsPullRequestApi()




## getTagsFilter()




## getTfsCollection()




## getTrackedFolderId()




## getUsername()




## getViewFormat()




## getWebLinkType()




## isAbsoluteRoot()




## isCommitsValidationRequired()




## isDisableSslVerification()




## isDisabled()




## isGitViewerEnabled()




## isGlobal()




## isHosted()




## isRefSpecChanges()




## isRefSpecNotes()




## isRequireUserPat()




## isSmartCommitsEnabled()




## isSourcesDiffViewEnabled()




## isTrustFolderStat()




## setAbsoluteRoot(Boolean)




## setApiFilter(String)




## setApiPath(String)




## setAwsRegion(String)




## setBranchLinkFormat(String)




## setChangesetFormat(String)




## setCommitsValidationRequired(Boolean)




## setCreateInitialCommit(Boolean)




## setDisableSslVerification(Boolean)




## setDisabled(Boolean)




## setDisplayName(String)
Sets the display name of the repository.<br>
This is the name that will appear in the Git Integration for Jira app repositories list.

`GIJFacade.createRepsitory()`: Optional. Autogenerated by default.
<br>
`GIJFacade.updateRepository()`: Optional.

### **Parameters**
* `displayName`: the new display name



## setEnableFetches(Boolean)




## setEncryptedPassword(EncryptedString)
Sets new password for the git repository. Leave blank and use PAT if 2FA is enabled on the git server.

 The IN password will be encrypted.
 Use `initPassword()` when none encryption is required.<br>
 [GIJFacade](/git-integration-for-jira-data-center/scriptrunner-javadoc-git-services-GIJFacade-gij-self-managed/) requires an [IntegrationRequest](/git-integration-for-jira-data-center/scriptrunner-javadoc-git-rest-integration-IntegrationRequest-gij-self-managed/) with an encrypted password, so use `setPassword()` instead of `initPassword()`.

### **Parameters**
* `password`: new password



## setEncryptedPat(EncryptedString)




## setFileAddedFormat(String)




## setFileDeletedFormat(String)




## setFileModifiedFormat(String)




## setFolderDepth(Integer)




## setGitViewerEnabled(Boolean)




## setGlobal(Boolean)




## setGroup(String)




## setHosted(Boolean)




## setId(Integer)




## setInitDate(Date)




## setIntegrationType(IntegrationType)




## setLastIndexedDate(Date)




## setMainBranch(String)




## setMaxMinsToCommitEmail(Integer)




## setMergeRequestFormat(String)




## setOrigin(String)




## setPassword(String)




## setPat(String)




## setProjectMappingIds(Set\<Long\>)




## setRealRoot(String)




## setRefSpecChanges(Boolean)




## setRefSpecCustom(String)




## setRefSpecNotes(Boolean)




## setRepositoryHostingUrl(String)




## setRepositoryKey(String)




## setRequireUserPat(Boolean)




## setRevisionIndexing(Boolean)




## setRoot(String)




## setSendCommitEmails(Boolean)




## setShowAllTags(Boolean)




## setSmartCommitsEnabled(Boolean)




## setSourcesDiffViewEnabled(Boolean)




## setSshKeyId(Integer)




## setSupportsBranchCreationApi(Boolean)




## setSupportsPullRequestApi(String)




## setTagsFilter(String)




## setTfsCollection(String)




## setTrackedFolderId(Integer)




## setTrustFolderStat(Boolean)




## setUsername(String)




## setViewFormat(String)




## setWebLinkType(String)




## toRepositoryTransformer(MultipleGitRepositoryManager)




## toShortFormRepositoryTransformer(MultipleGitRepositoryManager)





