---
title: Explore basic text mode for groupings in Workfront
description: Learn about text mode, camel case, and some basic text mode that you can use in your report groupings in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-08-12T00:00:00.000Z'
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
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
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
autotag-review: '2026-05-06T13:59:41.713Z'
---
# Explore basic text mode for groupings in Workfront

>[!PREREQUISITES]
>
>* [Understand reporting elements](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=en)
>* [Understand reporting components](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=en)
>* [Create a basic grouping](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=en)


>[!TIP]
>
>* To gain a more in depth understanding of text mode we recommend watching the recorded webinar event [Ask the Expert - Introduction to Text Mode Reporting](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), which is one hour in length.
>* To learn even more about text mode we recommend watching the [Advanced reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutorials, which together are five and a half hours in length.
>* Click here to access [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

In this video, you will learn:

* What text mode is 
* What camel case is 
* Some _text mode code blocks_ you can use in your report groupings 

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12&learn=on&enablevpops=0)

## "Understand basic text mode for groupings" activities

### Task - 4 parents grouping

The following text mode will group tasks based on up to four levels of parents, and leave parents that don't exist blank.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![A screen image showing project tasks grouped by 4 parents](assets/4-parents-grouping.png)


### Task - Percent complete grouping

The following text mode will group tasks based on their percent complete. Tasks will fall into one of the following categories when grouped:

* 0%
* 1% to 25%
* 26% to 50%
* 51% to 75%
* 76% to 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![A screen image showing project tasks grouped by percent complete](assets/percent-complete-grouping.png)

### Task - statusEquatesWith, then status

The following text mode will group tasks by statusEquatesWith, then by status.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![A screen image showing project tasks grouped by statusEquatesWith](assets/status-equates-with.png)


### Proof Approval - Group by project name

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![A screen image showing Proof approvals grouped by project name](assets/proof-approvals-grouped-by-project-name.png)


### Proof Approval - Group by document name

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![A screen image showing Proof approvals grouped by project name](assets/proof-approvals-grouped-by-doc-name.png)

