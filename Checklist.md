

**Migrate Jira First**

* Create a dummy Project (this Project should not be Migrated)
* Migrate all Jira Projects (exept the dummy project we just created), all Users, Groups, and all other Data
* Once all Data is migrated navigate to Navigate to URL:  
<Jira_URL>/secure/admin/SiteDarkFeatures!default.jspa
* Then enable three Dark Features with the following commands:
        <code>
        com.atlassian.jira.migration.export.all.filters
        com.atlassian.jira.migration.export.multiprojects.boards
        com.atlassian.jira.migration.dashboard-migration.feature.enabled
        </code>
* Click add 
* !ONLY  USE THESE FEATURES IN ONE MIGRATION!
* Run the Migration of the Dummy Project
* Disable the Dark Features 