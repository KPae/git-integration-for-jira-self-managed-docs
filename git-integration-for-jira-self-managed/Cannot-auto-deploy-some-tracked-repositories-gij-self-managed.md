---

title: Cannot auto-deploy some tracked repositories -- Specified origin is incorrect or not supported
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

## Problem

Git Integration for Jira application is not able to index repositories from a self-hosted GitLab or GitHub server.

## Diagnosis

List of repositories may load in the wizard correctly - but repositories are not indexed.
Logs contain a message similar to:

```java
Сan't auto-deploy a new repository http://gitlab-server.company.com/path/repository.git
com.bigbrassband.jira.git.exceptions.InvalidRemoteOperationException: Specified origin http://gitlab-server.company.com/path/repository.git is incorrect or not supported
```

## Cause

GitLab or GitHub permissions of the service user connecting Jira (via the Git Integration for Jira app) are not sufficient to view source code for the repository.

## Solutions

Grant sufficient access to the service account user in GitLab or GitHub:

*   See [GitLab permissions](https://docs.gitlab.com/ee/user/permissions.html) (Reporter is minimum required)

*   See [GitHub permissions](https://help.github.com/en/articles/access-permissions-on-github#personal-user-accounts) (Read for GitHub organizations or Collaborator for personal owned repositories is is minimum required).

<br>

<div class="bbb-callout bbb--info">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        <b>Contact Us</b><br>
        If you still have a question - reach out to our <a href='https://help.gitkraken.com/git-integration-for-jira-data-center/gij-self-hosted-contact-support/'>Support Desk</a> or email us at <a href='gijsupport@bigbrassband.com'>gijsupport@bigbrassband.com</a>.
    </div>
    </div>
</div>
<br>

<br>

## More articles about troubleshooting, workarounds and solutions

[Avoid OutOfMemory exceptions by configuring or memory allocation with Jira to accommodate large repositories](/git-integration-for-jira-data-center/Avoid-OutOfMemory-exceptions-by-configuring-or-memory-allocation-with-Jira-to-accommodate-large-repositories-gij-self-managed)

**Cannot auto-deploy some tracked repositories: Specified origin is incorrect or not supported** (this page)

[Connection Reset when Accessing the Database](/git-integration-for-jira-data-center/Connection-reset-when-accessing-the-database-gij-self-managed)

["Dangerous use of multiple connections" error on local database](/git-integration-for-jira-data-center/Dangerous-use-of-multiple-connections-error-on-local-database-gij-self-managed)

[Duplicate entry 0 for key PRIMARY exceptions in log](/git-integration-for-jira-data-center/Duplicate-entry-0-for-key-PRIMARY-exceptions-in-log-gij-self-managed)

[Error while reindexing - Java heap space / Object too large, rejecting the pack](/git-integration-for-jira-data-center/Error-while-reindexing-Java-heap-space-Object-too-large,-rejecting-the-pack-gij-self-managed)

[Gitolite integration: Why the Git integration app not see the master branch?](/git-integration-for-jira-data-center/Gitolite-integration--why-the-Git-integration-app-not-see-the-master-branch-gij-self-managed)

[Health Check\: Database Collation](/git-integration-for-jira-data-center/Health-check--database-collation-gij-self-managed)

[Indexing error - Too many open files](/git-integration-for-jira-data-center/Indexing-error-Too-many-open-files-gij-self-managed)

[Installation fails when installing manually](/git-integration-for-jira-data-center/Installation-fails-when-installing-manually-gij-self-managed)

[Jira index error: IndexNotFoundException: no segments\* file found](/git-integration-for-jira-data-center/Jira-index-error--IndexNotFoundException--no-segments-file-found)

[Malformed input or input contains unmappable characters](/git-integration-for-jira-data-center/Malformed-input-or-input-contains-unmappable-characters-gij-self-managed)

[Personal access token failing Azure DevOps integration with Not Authorized error](/git-integration-for-jira-data-center/Personal-access-token-failing-azure-devops-integration-with-Not-Authorized-error-gij-self-managed)

[Problems with shared home on Azure Storage](/git-integration-for-jira-data-center/Problems-with-shared-home-on-azure-storage-gij-self-managed)

[Pull request index error: org.json.JSONException](/git-integration-for-jira-data-center/Pull-request-index-error--JSONException-gij-self-managed)

[Repositories missing from Azure DevOps integration](/git-integration-for-jira-data-center/Repositories-missing-from-azure-devops-integration-gij-self-managed)

[Service proxy has been destroyed  exceptions in log](/git-integration-for-jira-data-center/Service-proxy-has-been-destroyed-exceptions-in-log-gij-self-managed)

[SQLException Incorrect string value in merge requests](/git-integration-for-jira-data-center/SQLException-'Incorrect-string-value'-in-merge-requests-gij-self-managed)

[SSH key file format is invalid](/git-integration-for-jira-data-center/SSH-key-file-format-is-invalid-gij-self-managed)

[TFS - Not Authorized exception when Jira works thru proxy](/git-integration-for-jira-data-center/TFS-Not-authorized-exception-when-Jira-works-thru-proxy-gij-self-managed)

[Unexpected exception parsing XML document from URL error in log](/git-integration-for-jira-data-center/Unexpected-exception-parsing-XML-document-from-URL-error-in-log-gij-self-managed)
