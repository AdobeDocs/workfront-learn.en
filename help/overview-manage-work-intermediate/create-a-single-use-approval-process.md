---
title: Create a global and a single-use approval process
description: Learn how to create a global and a single-use approval process on a project, task, or issue.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
autotag-review: '2026-05-05T19:20:03.459Z'
---
# Create a global and a single-use approval process

Approval processes on projects, tasks, and issues allow a project manager to get expert confirmation that the work has been done right before moving forward. The project manager can create an approval process for each situation (this is known as a single-use approval process) or choose from a list of possibly many approval processes that have been created previously to meet common needs (these are known as global, or existing, approval processes).

In either instance, when the object status changes to one specified in the approval process the approver is notified in various ways to review the work and approve or reject it. Given that the entire project may be paused waiting for an approval, approvers should be aware in advance that they may be called on for an approval. If an approver is out of the office for any reason they may delegate their approvals to a qualified substitute. See [Delegate tasks, issues, and approvals](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md) for details.

In this video, you will learn how to create a global approval process and a single-use approval process on a project, task, or issue.

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on&enablevpops=1)

>[!TIP]
>
>You can add a single use approval process for a project or task to a project template.

>[!NOTE]
>
>You can set up a single use approval on projects and issues in the same way as described for tasks in the video.

## How to apply automatic issue approvals in a request queue

If you want to set up automatic issue approvals in a request queue, these can only be done using a global issue approval process and are applied in a [!UICONTROL Queue topic]. 

When creating or editing a [!UICONTROL Queue topic], select the global approval process in the **[!UICONTROL Default Approval]** field.

![Image showing how to select a default approval process in a queue topic](assets/automatic-issue-approval-1.png)

You may need to edit the issue approval process to make sure **[!UICONTROL Previous status]** is not what the issue is set to when the approval is rejected. This is because the previous status is **[!UICONTROL New]**, and this is also the status that triggers the approval process, so it is the status it will be set to when approved. To avoid confusion when the issue approval is rejected, it's better to set the status to something like **[!UICONTROL Won't Resolve]**, or a custom status created for this purpose.

![Image showing changing the status to use when the issue is rejected](assets/automatic-issue-approval-2.png)


## Recommended tutorials on this topic

* [Delegate tasks, issues, and approvals](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Understand group-specific approval processes](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Create a request flow](/help/manage-work/request-queues/create-a-request-flow.md)

