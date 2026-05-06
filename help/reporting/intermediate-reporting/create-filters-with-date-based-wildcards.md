---
title: Create filters with date-based wildcards
description: Learn how and when to use date-based wildcards and how to build a filter based on the current date.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-06-27T00:00:00.000Z'
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
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
autotag-review: '2026-05-06T13:57:08.996Z'
---
# Create filters with date-based wildcards

In this video, you will learn how to:

* Know when to use date-based wildcards 
* Understand the difference between Workfront's two date-based wildcards 
* Add a date-based wildcard to a filter 
* Create a custom date using wildcards, attributes, operators, and modifiers 
* Create a custom date range using wildcards 

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on&enablevpops=0)


## "Create filters with date-based wildcards" activities


### Activity questions

1. How would you build the filter rule if you wanted issues that have a due date of yesterday or today? 
1. How would you build the filter rule to find projects that were due last week? 
1. The following filter rules are part of a task report you use regularly. What type of results would you get from this report?

![An image of the screen to create a task filter with a date-based wildcard](assets/date-wildcard-answer-1.png)

### Answers

1. Filter on the issue planned completion date between [!UICONTROL $$TODAY-1d] and [!UICONTROL $$TODAY].  
1. Filter on the project planned complete date between [!UICONTROL $$TODAYb-1w] and [!UICONTROL $$TODAYe-1w]. 
1. This report finds tasks assigned to you that aren't yet finished (in other words, have a percent complete less than 100), and that are overdue or due today. The filter rule for the planned completion date of the tasks says to look at tasks that have a due date that is equal to or before today's date.
