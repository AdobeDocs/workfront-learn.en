---
title: Create EXISTS filters for complex reporting
description: Learn what an EXISTS filter is, what it can do for you, and how you can build one from scratch. Plus see a lot of useful examples of EXISTS filters.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-18808
last-substantial-update: '2025-08-25T00:00:00.000Z'
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
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
autotag-review: '2026-05-06T02:08:32.688Z'
---
# Create EXISTS filters for complex reporting

EXISTS filters are advanced, text mode filters, which allow us to work around the 2 table/field jump limitation in a standard report builder. Or, they can be used to identify objects in the system that lack a specific relationship condition via NOTEXISTS. 

In this video you will learn how to create an EXISTS filter to see "Proof approvals on Current projects" in a proof approvals report.

For a more in-depth walkthrough on how EXISTS function, please see [Create complex Text Mode filters using EXISTS statements](https://experienceleague.adobe.com/en/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) documentation.

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## EXISTS Filter Examples

### Project Report EXISTS

This uses the task as the linking object, by comparing the projectID found at the task level and matching it to the project level ID field. This allows us to then compare the assignment users on the task to a $$USER.ID wildcard. This results in returning only projects where the viewing user is assigned to a 
task, regardless if they are the primary assignee or not.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


This uses the issue (optask) as the linking object, by also comparing the projectID found at the issue (optask) level and matching that to the project level ID field. This then checks to see if any of those issues (optasks) have an entry date within the span specified. In this case it would return any project that has 
not had an issue (optask) logged in a rolling past 30 days, due to the NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Template Report EXISTS

This filter will show all templates that have not been used to either create a project or have been attached to a project in the past year. One caveat is that in order to figure out whether or not a template was used as an attachment, it is dependent on that template having tasks in it.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### Task Report EXISTS

This uses the User table as the linking object, connecting by the assignments taskID and the tasks ID. This then checks the teams collection of IDs to the user Team IDs, returning the task if any of the assignees are on the same team as the viewing user.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### User Report EXISTS

This will return all users who have not posted an update in the past 3 weeks. This uses the note object to bridge the gap and compares the ownerID to a users ID. Then returns that user if no notes owned by them have an entry date greater than 3 weeks ago.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

This will return all users who have not logged hours in the last week. This uses an extremely similar method to the example above, but instead uses the hour owner info and hour entry date to base what users it returns.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

In a user report, show a list of users that matches a project's People's tab.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Category (Custom Form) Report EXISTS

This text will give you a list of all project forms that have not been used on a project at all, ever. This should be used in conjunction with specifying the object type of the form we are focused on. So in this case the focus is PROJ, so we should include the callouts in the objTypes lines. This could be used 
for other object types by changing the object code related parts. This checks the collection of projects attached forms, to the listed forms and returns if there is no match.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Parameter (Custom Field) Report EXISTS

This returns any custom field that is not currently attached to a custom form in the system. 

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Report Report EXISTS

This will return any report using a specific value in its filters.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

This will return any report that is attached to any dashboard.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### Proof Approval Report EXISTS

This would return proof approvals only on projects in a status of Current. This uses the Document object to bridge the gap from proof approval to project by checking the currentVersionID to the documentVersionID, from there we jump to the projects status. 

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
