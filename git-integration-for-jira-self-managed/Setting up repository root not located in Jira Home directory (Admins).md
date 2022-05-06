---
 
title: Setting up repository root not located in Jira Home directory (Admins)
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# Setting up repository root not located in Jira Home directory (Admins)

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1930396317>

* * *

There are three possible ways to setup a repository root that is not located in the Jira home directory:

1.  Clone the repository outside of Jira then connect to it via Manage git repositories page ➜ Connect to Git Repository ➜ **Advanced Setup**.
    
2.  Clone the repository with the standard **Connect to Git Repository** wizard into the Jira home directory.  Soon afterwards, move the cloned repository and update the settings on the repository.
    
3.  You could symlink the `{$JIRA_HOME}/data/git-plugin` directory to a different volume. The standard **Connect to Git Repository** wizard will still write there, but the data will reside on the different volume. But be aware, that the Git Integration for Jira app treats anything in the `git-plugin` folder as a clone that it owns.
    

[« Adding a repository hosted on Windows Servers or Windows Network Share (Admins)](/wiki/spaces/GIJDC/pages/1930396287)

[Reindex API to trigger indexing »](/wiki/spaces/GIJDC/pages/1930396333/Reindex+API+to+trigger+indexing)

### More related topics about getting started for git admins

*   Page:
    
    [Setup GitLab Server to respond to incoming network API calls](/wiki/spaces/GIJDC/pages/1930396193/Setup+GitLab+Server+to+respond+to+incoming+network+API+calls) (Git Integration for Jira Data Center)
    
*   Page:
    
    [New GitLab v10+ authentication](/wiki/spaces/GIJDC/pages/1930396211) (Git Integration for Jira Data Center)
    
*   Page:
    
    [General settings: Improving Jira performance](/wiki/spaces/GIJDC/pages/1930396229/General+settings%3A+Improving+Jira+performance) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Adding a repository hosted on Windows Servers or Windows Network Share (Admins)](/wiki/spaces/GIJDC/pages/1930396287) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up repository root not located in Jira Home directory (Admins)](/wiki/spaces/GIJDC/pages/1930396317) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Recommended reindex interval setting](/wiki/spaces/GIJDC/pages/1930396353/Recommended+reindex+interval+setting) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Reindex API to trigger indexing](/wiki/spaces/GIJDC/pages/1930396333/Reindex+API+to+trigger+indexing) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up web linking](/wiki/spaces/GIJDC/pages/1930396395/Setting+up+web+linking) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up webhooks](/wiki/spaces/GIJDC/pages/1930396415/Setting+up+webhooks) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Increasing timeout threshold for large repositories while doing a Git pull](/wiki/spaces/GIJDC/pages/1930396447/Increasing+timeout+threshold+for+large+repositories+while+doing+a+Git+pull) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Working with Tracked folders](/wiki/spaces/GIJDC/pages/1930396479/Working+with+Tracked+folders) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Recommended upgrade method for Git Integration for Jira](/wiki/spaces/GIJDC/pages/1930396509/Recommended+upgrade+method+for+Git+Integration+for+Jira) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Discard cloned files in Jira Home directory (General setting)](/wiki/spaces/GIJDC/pages/1930396547) (Git Integration for Jira Data Center)