---
title: Set up Reminder Notifications
description: Learn how to set up object-specific reminder notifications to let users know when work is due soon or overdue.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
TQID: https://experienceleague.adobe.com/sfd4zrfrTkqEfkO5cPL85ZiD-RawPbikiUQO5oq-nuc
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
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
<!--
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
-->

# Set up reminder notifications

Reminder notifications are created by system administrators in the [!UICONTROL Setup] area. Then they can be attached and used by project, task, and issue owners as reminders for when work is due soon or overdue. 

Reminders are object-specific and have to be manually attached to the corresponding work item so the notification can be sent.

**Create a reminder notification**

1. Click **[!UICONTROL Setup]** in the **[!UICONTROL Main Menu]**.
1. Click the **[!UICONTROL Email]** section.
1. Click the **[!UICONTROL Notifications]** section.
1. Click the **[!UICONTROL New Reminder]** tab. 
1. Click the **[!UICONTROL +New Reminder Notification]** button.
1. Select the desired object for the drop-down menu.
1. Fill in the required information.
1. Click **[!UICONTROL Save]**.

![[!UICONTROL New Reminder Notification] window](assets/admin-fund-reminder-notification-1.png)

When setting up the reminder, there are a few things to consider:

* **[!UICONTROL Reminder Notification Name] —** This is the name that will be seen by project managers when they attach a reminder to an object. Make sure the name is succinct but descriptive.
* **[!UICONTROL Qualifying Period] —** The number of hours, days, weeks, or months before/after the date selected in the Timing section.
* **[!UICONTROL Timing] —** Select whether the reminder should be sent before or after the object’s planned, projected, or actual start/completion dates. Options for timesheets are related to the start date, end date, or last update date.
* **[!UICONTROL Criteria] —** Specify the criteria to qualify the reminder to be sent. Options vary depending on the object-specific reminder. 
* **[!UICONTROL Recipients] —** Select who the reminder should be sent to. The stakeholder options vary depending on the object type selected for the reminder.
 
Once the reminder settings have been established and saved, the reminder notification is available to object owners to use within [!DNL Workfront].

## Email customization

Reminder notifications use a default email format and message. If you want to customize the email, you can create a template.

<!--
paragraph above needs a hyperlink to an article
-->

![New Email Template window](assets/admin-fund-email-customization.png)

<!--
learn more URLs
-->
