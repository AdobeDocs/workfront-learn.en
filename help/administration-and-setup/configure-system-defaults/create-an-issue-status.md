---
title: Create an Issue Status
description: Learn how to create an issue status to meet the needs of your organization's workflows.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
TQID: https://experienceleague.adobe.com/lbk5pXw2QHyOdFKDSIE8xCAdpIPBHvdJXsG5ui7H7JM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create an issue status

[!DNL Workfront] recommends you modify existing issue statues in your system before you start creating new statuses. This helps limit the number of statuses that need to be maintained.

1. Click **[!UICONTROL Setup]** in the **[!UICONTROL Main Menu]**.
1. Expand the **[!UICONTROL Project Preferences]** section in the left menu panel.
1. Select **[!UICONTROL Statuses]**.
1. Select the **[!UICONTROL Issues]** tab.
1. Make sure the field in the upper-right is set to [!UICONTROL System Statuses]. This ensures the new status is available globally across your [!DNL Workfront] instance.
1. Select **[!UICONTROL Master List ]** to see all issue statuses. This is where you create or modify a status.
1. Click **[!UICONTROL Add a New Status]**.
1. Complete the fields as needed for your organization — name, description, color, equates with, key, etc.
1. Check the boxes for the type of issue this status can be used with.
1. Click **[!UICONTROL Save]**.

![New status window on [!UICONTROL Statuses] page](assets/admin-fund-create-issue-status.png)

## Issue statuses and group administrators

Group administrators can create and customize issue statuses for the groups they manage. This provides some autonomy for their group, providing them with the statuses they need to keep work moving. It also eliminates the need for a long list of system-wide statuses.

Group administrators can edit existing statuses if the system administrator has configured them to allow customization.

System administrators can manage statuses for groups by selecting the group name in the upper-right corner of the [!UICONTROL Statuses] window.

![Group list menu on [!UICONTROL Statuses] page](assets/admin-fund-change-group-master-list.png)

Group administrators can click into the [!UICONTROL Groups] section in the [!UICONTROL Setup] area, open their group by clicking the name, and then selecting [!UICONTROL Statuses] in the left panel menu. Be sure to select the Issues tab.

![[!UICONTROL Statuses] section of [!UICONTROL Group] page](assets/admin-fund-group-issue-statuses.png)

<!--
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
-->

<!--
learn more URLs
Issue statuses
Create and customize system-wide statuses
-->
