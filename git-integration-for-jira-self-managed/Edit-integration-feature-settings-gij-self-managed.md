---

title: Edit integration feature settings
description:
taxonomy:
    category: git-integration-for-jira-data-center

---

Clicking <img src='/wp-content/uploads/actions-icon.png' /> Actions ➜ **Edit integration feature settings** opens the configuration page for integration features settings such as repository browser, requiring user PAT, project permissions and more.

![](/wp-content/uploads/gij-gitcfg-actions-edit-feature-conn-cfg.png)

&nbsp;

Utilize the following options to configure the selected integration:

- [Repository Browser](#repository-browser)
- [Tags](#tags)
- [Personal Access Token: Require User PAT](#personal-access-token-require-user-pat)
- [Project Permissions](#project-permissions)
- [Source Code Diff Viewing](#source-code-diff-viewing)
- [Smart Commits](#smart-commits)
- [Commit Notification Emails](#commit-notification-emails)

&nbsp;
* * *
&nbsp;

### Repository Browser

<img src='/wp-content/uploads/gij-gitserver-edit-repocfg-repovw.png' style='display:block;margin:25px auto;max-width:100%' />

When `Enabled`, it allows users to view Git repositories of configured projects. For more information, see [Repository Browser](/git-integration-for-jira-data-center/repository-browser-gij-self-managed/).

&nbsp;

### Tags

<img src='/wp-content/uploads/gij-gitserver-edit-features-tags.png' style='display:block;margin:25px auto;max-width:100%' />

Set whether to show all tags or show on tags with matching regex pattern. For more information on git tags, see [Git Tags](/git-integration-for-jira-data-center/git-tags-gij-self-managed/).

&nbsp;

### Personal Access Token: Require User PAT

<img src='/wp-content/uploads/gij-gitserver-edit-features-pat-reqpat.png' style='display:block;margin:25px auto;max-width:100%' />

Enable this option to require users to provide PAT which will be used for branch and merge/pull request creation/deletion (via the developer panel on the Jira issue page). This is a security feature of Git Integration for Jira app for git hosts that support two-factor authentication.

<div class="bbb-callout bbb--alert">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        This option requires the <a href='/git-integration-for-jira-data-center/repository-browser-gij-self-managed'>Repository Browser</a> feature enabled.
    </div>
    </div>
</div>

<div class="bbb-callout bbb--info">
    <div class="irow">
    <div class="ilogobox">
        <span class="logoimg"></span>
    </div>
    <div class="imsgbox">
        This setting is only available for auto-connected git hosts in Jira Server and Jira Data Center.
    </div>
    </div>
</div>

&nbsp;

### Project Permissions

<img src='/wp-content/uploads/gij-gitserver-edit-feature-cfg-proj-acls.png' style='display:block;margin:25px auto;max-width:100%' />

The default setting is **Associate with all projects**. You can restrict access to the Repository Browser and Git Commits tabs for the selected repository by setting the project associations.

To restrict to specific projects, uncheck the **Associate with all projects** _option_ and set/select one or more projects from the list.

&nbsp;

### Source Code Diff Viewing

<img src='/wp-content/uploads/gij-gitserver-edit-features-src-code-diffvw.png' style='display:block;margin:25px auto;max-width:100%' />

Allows or denies users to view the diff by commit and file.

&nbsp;

### Smart Commits

<img src='/wp-content/uploads/gij-gitserver-edit-features-smartcommits.png' style='display:block;margin:25px auto;max-width:100%' />

Allows or denies the users to use the smart commits feature.

&nbsp;

### Commit Notification Emails

<img src='/wp-content/uploads/gij-gitserver-edit-features-commit-notif-emails.png' style='display:block;margin:25px auto;max-width:100%' />

Enable/disable this setting to allow/deny sending of commit notification emails.

Set the **Max commit age (in minutes)** as to when commit notifications will be sent. Commit notifications will be e-mailed if the age of the commit is less than or equal to this value.

&nbsp;
* * *

[**Prev:** Edit integration connection settings](/git-integration-for-jira-data-center/edit-integration-connection-settings-gij-self-managed)

[**Next:** Edit repository settings](/git-integration-for-jira-data-center/edit-repository-settings-gij-self-managed)

