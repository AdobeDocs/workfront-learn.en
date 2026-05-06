---
title: Understand navigating and reviewing projects
description: Learn how to read the Flight plan chart in [!UICONTROL Enhanced analytics].
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8729
recommendations: noDisplay,catalog
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
<<<<<<< Updated upstream
TQID: https://experienceleague.adobe.com/poXtsec8RB-p09xumOQTblOqqx2VNvTTLv7blMggz8U
=======
>>>>>>> Stashed changes
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
<<<<<<< Updated upstream
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
=======
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
subfeature_v2:
  - id: db1e0ccb-6619-410a-84d6-6b80ac783274
    internal-label: Enhanced analytics
>>>>>>> Stashed changes
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
<<<<<<< Updated upstream
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
=======
autotag-review: '2026-05-06T14:11:51.971Z'
>>>>>>> Stashed changes
---
# Understand navigating and reviewing projects

In this video, you will learn:

* How to read the Flight plan chart

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on&enablevpops=1)

## Flight plan chart

![An image of a flight plan chart with numbers matching bullets below](assets/section-2-1.png)

On the chart, you see:

1. Project names are on the left.
1. Dates are shown across the bottom. 
1. The vertical blue line shows the specific date where your mouse is hovering. 
1. Horizontal blue lines show the planned start and end dates of the project.
1. Green lines indicate the project is On Target.
1. Orange lines indicate the project is At Risk. 
1. Red lines indicate the project is In Trouble. 

Seeing this information about your projects helps you determine:

* What events extend a project past the planned completion date.
* When a project starts to run into issues.
* How many projects are open over the same time period.
* How many projects are active.
* Which projects need extra attention or support.

## Condition is based on progress status

The project condition is a visual representation of how the project is progressing. Workfront determines the condition based on progress status of tasks within the project.

![An image of possible progress statuses](assets/section-2-2.png)

The condition of a project can be set:

* **Manually**, by users with access to manage the project, when the project's condition type is set to manual. This allows you to set the condition of the project independently from the critical path.
* **Automatically**, by Workfront, when the condition type of the project is set to Progress Status.

Workfront recommends that you set the condition type to Progress Status so you have a clear indication of the true progress of the project, based on the progress of your tasks.

![An image of possible progress statuses](assets/section-2-3.png)

When set to Progress Status, the project condition can be:

* **On Target**—When the progress status of the last task on the critical path is On Time, the condition of the project will be On Target. The project is on track to finish on schedule.
* **At Risk**—When the progress status of the last task on the critical path is Behind or At Risk, then the condition of the project is At Risk. The project is on track to finish late but isn't late yet.
* **In Trouble**—When the progress status of the last task on the critical path is Late, then the condition of the project is In Trouble. The due date is in the past and the project is now late.

>[!NOTE]
>
>Conditions can be customized for your environment, so you may find more than three options or the names may be different than the ones above. For information about customizing conditions, see the article [Create or edit a custom Condition](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-conditions/create-edit-custom-conditions.html?lang=en).
