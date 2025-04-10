---
title: Track progress from the project timeline
description: Learn how to track the progress of work from the project timeline in [!DNL  Workfront] using percent complete, status, assignments, or constraints.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16
level: Beginner
jira: KT-10150
hide: yes
---
# Track progress from the project timeline

Make sure tasks are progressing the way they should to hit project deadlines. As you scan through the [!UICONTROL Task] list, there are several features in [!DNL  Workfront] that help you monitor the progress and status of work.

## Percent complete

The percent complete on each working task is sometimes used to gauge how work is progressing. It's important to note...this field has to be adjusted manually, as it's the assignee's estimation of how far along they are.

>[!TIP]
>
>Although percent complete on working tasks needs to be updated manually, the percent complete of a parent task is calculated by Workfront based on the percent complete and either the duration or planned hours of each child task. What this means is that you'll get better percent complete accuracy if you break large tasks into smaller subtasks.


![Project task list showing [!UICONTROL Percent Complete] column](assets/planner-fund-task-percent-complete.png)

There are three times when the percent complete changes automatically:

* When the task [!UICONTROL Status] is set to Complete, the percent complete changes to 100.
* If the task [!UICONTROL Status] rolls back to New, the percent complete is reset to 0.
* In a parent task when the percent complete of a child task changes.

## Status

Include the [!UICONTROL Status] column in a [!UICONTROL View] to quickly see which tasks have been started, which are in progress, and which are complete. You can even set up conditional formatting in a [!UICONTROL View] to color code each status, making the information easier to decipher.

## Task assignments

As you review the project, review the task assignments. Maybe work fell behind because no one was assigned to the task. Or maybe the person assigned didn't have the right skill set to complete the work. Add more people to a task or reassign tasks to ensure work gets done.

## Task constraint

Sometimes task constraints get changed and you don't realize it. Constraints can affect how your timeline behaves, so you should make sure they're set how you want them.

![Project task list showing task constraint column](assets/planner-fund-task-constraint.png)

Create a custom view that includes the [!UICONTROL Task Constraint] column to see this information on your task list. If you planned the project from a start date, you want your tasks to have the [!UICONTROL As Soon As Possible] ([!UICONTROL ASAP]) constraint.

For more details about task constraints see [Understand and manage duration types and task constraints](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).
