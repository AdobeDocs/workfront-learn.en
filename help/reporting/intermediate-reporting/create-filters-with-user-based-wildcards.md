---
title: Create filters with user-based wildcards
description: Learn how to use user-based wildcards and how to build a filter based on the logged in user.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-06-26T00:00:00.000Z'
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
subfeature_v2:
  - id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
    internal-label: Create and manage reports
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
autotag-review: '2026-05-06T13:58:26.659Z'
---
# Create filters with user-based wildcards

In this video, you will learn how to:

* Understand why to use wildcards 
* Build a filter with a user-based wildcard 

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on&enablevpops=0)

>[!TIP]
>
>Use the Assignment Users >> ID field source and name when building filters that look at task or issue assignment information.  This option looks at all of the users assigned to the task or issue, not just the "owner" or primary assignee. 

>[!TIP]
>
>Use the $$USER.ID (instead of your name) even when building filters for yourself. This way, if someone sees a filter you're running and says "share that with me," the filter is already set up so each person using it sees their own information. 

>[!TIP]
>
>You always must use the Equal filter qualifier when using user-based wildcards. 


## "Create filters with user-based wildcards" activities

### Activity 1

You have a bit of extra time this week, so you want to see if there's anyone on your team who could use some assistance with their assignments. Create a task filter to find tasks assigned to your home team that are due this week and haven't been completed yet.  

### Answer 1

You're awesome for helping out your teammates! With the filter set up like the image below, you'll find tasks: 

* That haven't been completed (meaning they don't have a [!UICONTROL Complete] status or status that equates to [!UICONTROL Complete]); 
* That are in projects with a [!UICONTROL Current] status (after all, you don't want to find tasks for projects that haven't launched yet); 
* That are assigned to someone on your home team, as defined by Workfront team settings; 
* And that have a completion date of sometime this week (this rule used the pre-built date filter to define "this week"). 

![An image of the screen to create a task filter with a user-based wildcard](assets/user-wildcard-exercise-answer.png)

You may need to add some additional filters if you need to limit the list a bit more. For example, you may want to add a filter rule that looks at a specific program or portfolio that your team works out of.
