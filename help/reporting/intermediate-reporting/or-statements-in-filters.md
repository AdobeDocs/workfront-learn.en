---
title: Create OR statements in filters
description: Workfront's flexible filter logic allows users to refine reporting views using default "AND" rules, optional "OR" conditions, and organized filter groups for complex criteria.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11
doc-type: video
---
# Create OR statements in filters

The video explains how to create and use filters with multiple rules in Workfront. ​ By default, Workfront uses "AND" between filter rules, meaning all conditions must be true for an item to appear in the list.
Alternatively, you can change the filter logic to "OR," which displays items that meet any of the conditions. 
The video also demonstrates creating filters for tasks using filter groups. ​ For example, you can create two groups: one for incomplete tasks assigned to the creative team that are late, and another for incomplete tasks assigned to the creative team that are unassigned. ​ Within each group, "AND" logic applies, meaning all conditions in the group must be met. ​ The "OR" logic between groups ensures tasks meeting the conditions of either group are displayed. 

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0)

## OR filter activity

You want to find incomplete tasks that are assigned to you or that aren't assigned to anyone. You set up a filter to look like the one below. Will this filter give you the results you want? Why or why not? 

![An image of an improperly created OR statement in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Answers 

No, this filter will not provide the results you're hoping for—tasks that aren't finished that are either assigned to you or assigned to no one—because the filter rule for the task completeness is only on one side of the OR. 

Instead, this filter will generate a list that shows: 

* Tasks assigned to you that are not complete. 
* **PLUS (OR)** 
* All unassigned tasks, no matter what the status is. 

The filter should look like the one below. Notice this filter has the filter rule for task completeness on both sides of the OR. 

![An image of a properly created OR statement in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
