---
title: Apply an issue approval process in a request queue
description: Implement a default approval process to streamline request workflows, ensuring approved requests change their status appropriately to "New." Address confusion for rejected requests by selecting a status change to "Won't Resolve."
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
<<<<<<< Updated upstream
last-substantial-update: 2025-03-26T00:00:00.000Z
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
TQID: https://experienceleague.adobe.com/PuiOlZeF17pZ23e6JHYWIvVvMawUiYHrIhVEYTPs8UQ
=======
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
>>>>>>> Stashed changes
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
<<<<<<< Updated upstream
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
=======
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
>>>>>>> Stashed changes
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
<<<<<<< Updated upstream
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
=======
autotag-review: '2026-05-06T15:58:59.618Z'
>>>>>>> Stashed changes
---
# Apply an issue approval process in a request queue

>[!PREREQUISITES]
>
>* [Create a request flow](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Create a global and a single-use approval process](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


The video explains the process of applying a default approval process when creating a request queue. ​ When a request is created, it starts with the status "New - Pending Approval," and an approval notification is sent to the designated approver. ​ If approved, the status changes to "New," allowing assigned individuals to begin work. ​ If rejected, the status may incorrectly revert to "New" due to a common mistake in the approval process setup. ​
The video highlights that the approval process is triggered when the status is set to "New," which is the default for new requests. ​ If rejected, the system defaults to changing the status back to the previous one, which is not ideal for new requests. ​ Instead, a different status, such as "Won't Resolve," should be chosen. ​ The video also notes that there is no "Rejected" status provided by default, but a system administrator can create one if needed. ​

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## Key takeaways

* **Default Approval Process:** When creating a request queue, you can apply a default approval process that automatically assigns an approval workflow to each request.
* **Status Changes Upon Approval:** Approved requests change their status from "New - pending approval" to "New," allowing assigned individuals to start working on them.
* **Common Mistake in Rejection Handling:** If a request is rejected, the status will revert to "New" due to a default system setting in the approval process.
* **Recommended Status for Rejected Requests:** Instead of reverting to the previous status ("New"), it is better to choose a different status, such as "Won't Resolve," to avoid confusion.
* **Custom Status Options:** There is no "Rejected" status provided by default, but a system administrator can create one if needed for better clarity in the approval process.


## Recommended tutorials on this topic

* [Delegate tasks, issues, and approvals](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Understand group-specific approval processes](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Create a request flow](/help/manage-work/request-queues/create-a-request-flow.md)
* [Create a global and a single-use approval process](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
