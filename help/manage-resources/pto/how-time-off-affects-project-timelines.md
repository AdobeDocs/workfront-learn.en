---
title: Show time off affects project timelines
description: See what happens to a project timeline when the time off setting is on and off.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
TQID: https://experienceleague.adobe.com/sN6HqoLl6N-asOtCSlZyKP6W0FSpT0C-7egQTlgAdkY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
---
# How time off affects project timelines

Whether an assigned user’s time off factors into the project timeline depends on a project setting called [!UICONTROL User Time Off]. This setting determines if the time off for the primary assignee of the task adjusts the planned dates for that task on the project.

Let’s look at what happens with a project timeline when each of the settings is selected—C[!UICONTROL onsider user time off in task durations] or [!UICONTROL Ignore user time off in task durations].

![User time off setting](assets/toapt_01.png)

## Consider user time off in task durations

This option is Workfront’s default setting.

In this example, the primary assignee for the task has days off marked on their personal calendar.

![personal calendar](assets/toapt_02.png)

The project manager wants to assign this person to a task that has planned dates that overlap the user’s time off.

![project task with dates](assets/toapt_03.png)

When this user is assigned to the task, the planned dates adjust automatically. Now the task’s planned completion date has extended by several days to accommodate the user’s time off. It’s important to note this change can affect the planned dates of other tasks in the project and, potentially, the project’s planned completion date.

![project task with due date](assets/toapt_04.png)

## [!UICONTROL Ignore user time off in task durations]

With this option, the planned dates of the task remain as originally planned, even if the primary assignee has time off during the duration of that task.

The team member has days off marked on their calendar.

![pto calendar with marked off dates](assets/toapt_05.png)

The project manager assigns them a task that overlaps the time off. Once the user is assigned, the task planned dates remain as originally planned.

![adjust project task dates](assets/toapt_06.png)

To ensure the work gets done on time, it might be helpful to assign another person who can work on the task while the original assignee is out of the office.

## Adjust the setting at the project level

To change the User Time Off setting on a project:

* Open the project by clicking its name in Workfront.

* Select [!UICONTROL Edit] from the 3-dot menu in the page header, to the right of the project name.

* Scroll to the [!UICONTROL Project Settings] section and find the [!UICONTROL User Time Off] field.

* Select the option you want to apply to this project — [!UICONTROL Consider user time off in task durations] or I[!UICONTROL gnore user time off in task durations].

* Click the [!UICONTROL Save] button in the upper-right corner of the window.

![Consider user time off in task durations](assets/toapt_07.png)


**Note**: This setting is not available when you select [!UICONTROL Project Details] from the left panel menu of the project page.

A global setting for this exists in the project preferences in the [!UICONTROL Setup] menu. This setting is managed by your system administrator. Group administrators may be able to adjust this setting for the groups they manage.

Workfront recommends the setting be set the way you want the majority of your projects to handle time off at your organization.

The setting also can be built into project templates, through the template details.
