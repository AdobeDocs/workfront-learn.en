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
last-substantial-update: 2025-03-26
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
---
# Apply an issue approval process in a request queue

>[!PREREQUISITES]
>
>* [Create a request flow](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Create a global and a single-use approval process](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


The video explains the process of applying a default approval process when creating a request queue. ​ When a request is created, it starts with the status "New - Pending Approval," and an approval notification is sent to the designated approver. ​ If approved, the status changes to "New," allowing assigned individuals to begin work. ​ If rejected, the status may incorrectly revert to "New" due to a common mistake in the approval process setup. ​
The video highlights that the approval process is triggered when the status is set to "New," which is the default for new requests. ​ If rejected, the system defaults to changing the status back to the previous one, which is not ideal for new requests. ​ Instead, a different status, such as "Won't Resolve," should be chosen. ​ The video also notes that there is no "Rejected" status provided by default, but a system administrator can create one if needed. ​

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

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
