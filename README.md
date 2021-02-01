# MS_Teams

## Overview
Repo for all Graph API or Powershell cmdlet integrations with the O365 and Azure tenants.

## In Production
#### MS Teams - Add/Remove Member Automation

Script that will add and remove users from defined Teams based on Team and AD Group membership. This integration is dependent on the "teams.yml" configuration file. 
##### Notes for Teams
If a new Team is created and want to automate the adding and removing of users, you will need to add the "team" name using the exact mailbox name as found in the Azure AD Groups. This can be found by logging into the Azure Portal (admin rights required), or using the Microsoft Graph API Explorer. When creating a new Team, **make sure that create a new AD group that is exclusive to that team**
##### Notes for Groups
If any additional AD groups need to be associated with a Team, the exact name of that AD Group will need to be added to the "teams.yml" file as a "group". If an individual user needs to be added to the Team, add them to the exclusive "team_xxxx" security group in AD that should have been created when creating a new Team.


## In Development
