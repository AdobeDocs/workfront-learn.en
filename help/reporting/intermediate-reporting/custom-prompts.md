---
title: Create custom prompts using text mode
description: Learn what a custom prompt is, how to create a custom prompt using text mode, and some examples that you can use in reporting in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-05T00:00:00.000Z
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
TQID: https://experienceleague.adobe.com/5l7BrwZPMI7o9mJeITi6Yf93fu5CB4w2k2eS-yeL290
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
---
# Create custom prompts using text mode

In this video, you will learn:

* What a custom prompt is  
* How to create a custom prompt using text mode  
* Some examples that you can use in your reporting 

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0)

## "Create custom prompts" activities


### Activity: Create custom prompts

1. Create a custom prompt that shows the following project statuses in the prompt drop-down menu:
   * Planning 
   * Current 
   * Completed 
   * Dead 
1. Modify the prompt to show current projects that are due this month. 
 
### Answers 

1. Your custom prompts should look similar to this and have the following text mode: 

   ![An image of the screen to create a new filter in text mode](assets/cp-01.png)

   Once you save the custom prompt, the prompt drop-down menu should look like this: 

1.  The text mode in your custom prompt should look like this: 

   ![An image of the screen to create a new filter in text mode](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

   And the drop-down label for active prompts should be updated to reflect the change in the code like this: 

   ![An image of the screen to create a new filter in text mode](assets/cp-02a.png)
