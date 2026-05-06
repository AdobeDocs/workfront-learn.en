---
title: Explore basic text mode for filters in Workfront
description: Learn about text mode, camel case, and some basic text mode that you can use in your report filters in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
<<<<<<< Updated upstream
last-substantial-update: 2025-07-30T00:00:00.000Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
TQID: https://experienceleague.adobe.com/vSZ-gnpBU32S-7SUyTHgIgqvAgaAFYyHZ4S1lKFqiJg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
=======
last-substantial-update: '2025-07-30T00:00:00.000Z'
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
    internal-label: Text Mode reporting
>>>>>>> Stashed changes
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
<<<<<<< Updated upstream
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
=======
autotag-review: '2026-05-06T13:59:16.164Z'
>>>>>>> Stashed changes
---
# Explore basic text mode for filters in Workfront

>[!PREREQUISITES]
>
>* [Understand reporting elements](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=en)
>* [Understand reporting components](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=en)
>* [Create a basic filter](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=en)


>[!TIP]
>
>* To gain a more in depth understanding of text mode we recommend watching the recorded webinar event [Ask the Expert - Introduction to Text Mode Reporting](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), which is one hour in length.
>* To learn even more about text mode we recommend watching the [Advanced reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutorials, which together are five and a half hours in length.
>* Click here to access [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


In this video, you will learn about:

* Text mode
* Camel case
* Some _text mode code blocks_ you can use in your report filters

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on&enablevpops=0)

## "Understand basic text mode for filters" activities


### Task - Filter out tasks where I've marked "Done with my part"

The following text mode will exclude tasks where a user has marked "Done with My Part." All you have to do is create a task filter, add any filter rules you want, then switch to text mode and paste the code below after any text mode you see in the filter.


>[!WARNING]
>
> This is not intended for use in Calendar filters.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Task - Show me all tasks awaiting my approval

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Task - Show me all tasks I have approved

Create a task report with whatever filters you want, then go to the Filter tab and click on Switch to Text Mode. Add this code to whatever is already there:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Task - Show me all tasks that have at least one cross project predecessor

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Task - Show me all tasks I assigned to others

Create a task report with whatever filters you want, then go to the Filter tab and click on Switch to Text Mode. Add this code to whatever is already there:

>[!WARNING]
> 
> This is not intended for use in Calendar filters.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

This will show you all tasks where the logged in user assigned at least one of the current assignees. If assignees were assigned by multiple people only the name of the first person who assigned someone will appear as "Requested By" on the task landing page.

### Task - Show me all tasks that are Complete - Pending Approval

```
status=CPL:A
status_Mod=in
```


### Issue - Show me all issues that are Complete - Pending Approval

```
status=CPL:A
status_Mod=in
```


### Project - Show me all projects that are Complete - Pending Approval

```
status=CPL:A
status_Mod=in
```


### Note - Show me all comments I'm tagged in

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Parameter/Custom Field Report - Show me custom fields that are not attached to a custom form (very useful in cleanup efforts)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
