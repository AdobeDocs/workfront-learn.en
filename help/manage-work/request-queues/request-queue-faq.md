---
title: Answers to common questions about request queues
description: Get answers to common questions about request queues in [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2024-09-16
recommendations: noDisplay,noCatalog
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
---
# Answers to common questions about request queues

**Why can I see a request queue, but my user cannot?**

In the [!UICONTROL Queue Details] tab of your request queue/project, ensure your user fits the criteria of the "Who can add requests to this queue?" field.

Watch this video for more details: 

>[!VIDEO](https://video.tv.adobe.com/v/3434156/?quality=12&learn=on)

**I gave users access to the queue, but now they can also see the request queue project. Why?**

In the "Who can add requests to this queue?" list, if you chose "People with view access to this project" then anyone you give view rights to for the sake of using the request queue will also be able to view the request queue in a project list. To avoid this, use the "People in this project's company" or the "People in this project's group" option.

**Can I turn a request into a project?**

Yes. You can convert issues into tasks or projects depending on what is needed.

These tutorials will show you how:

* [Convert an issue/request to a project](help/manage-work/issues-requests/create-a-project-from-a-request.md)

* [Convert an issue/request to a task](help/manage-work/issues-requests/convert-issues-to-other-work-items.md)

**Where do I find a request queue to make edits?**

You can use the [!UICONTROL Search] field in the navigation bar or find it listed in the [!UICONTROL Projects] area.

If you open a request from the request queue you can click on the project name in the breadcrumbs area.

**Can I transfer the information from a request custom form to a project custom form?**

Yes. When you create a custom form select both [!UICONTROL Project] and [!UICONTROL Issue] as the object types. You can also edit a project custom form to include the issue object type and vice versa. 

Attach the custom form to the request. When you convert the request to a project the custom form will automatically attach to the new project and the values contained in any fields will appear in both the request and the project custom forms.

**I'm looking at a project or task report. How can I find out what request this object originated from?**

You can access fields in the **[!UICONTROL Converted Issue]** and the **[!UICONTROL Converted Issue Originator]** field sources to add that information to your project and task reports.

Watch this video for more details: 

>[!VIDEO](https://video.tv.adobe.com/v/3434176/?quality=12&learn=on)


**What's the best way to filter for request queues in a report?**

If your project filter includes **Queue>>Is Public>>Equal>>None** your report will show only projects that are **NOT** request queues.

If your project filter includes **Queue>>Is Public>>Not Equal>>None** your report will show only projects that **ARE** request queues.

Watch this video for more details:

>[!VIDEO](https://video.tv.adobe.com/v/3434329/?quality=12&learn=on)

**Is it a good idea to create a custom status of Request Queue?**

Some customers create a custom status of Request Queue that equates with Current. They can then run a report showing all request queues or easily exclude request queues from a report. While this has the advantage of being more user friendly than using **Queue>>Is Public>>Not Equal>>None**, it has the disadvantage that people creating request queues may forget to use it, since the Current status works just as well and is what they'll see in most of the training material. For that reason many customers choose not to use a custom status of Request Queue.

However, if you're already using the Request Queue status in your organization and you just want a way to make sure it's being used properly (or fix cases where it isn't), you can create the **Active request queues** report described in the video above, and change the filter for **Project>>Status Equates With>>Equal>>Current** to **Project>>Status>>Equal>>Current**. This will show you all active request queues that are using the Current status instead of the Request Queue status you want them to use. Select all the projects that appear and do a bulk edit to change the statuses to Request Queue.

## Recommended tutorials on this topic

* [Understand request queues](/help/manage-work/request-queues/understand-request-queues.md)
* [Create a request queue](/help/manage-work/request-queues/create-a-request-queue.md)
* [Understand settings for a request flow](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)
* [Create a request flow](/help/manage-work/request-queues/create-a-request-flow.md)
* [Create a system admin feedback request queue](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
