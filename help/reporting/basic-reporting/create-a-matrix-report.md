---
title: Create a matrix report
description: Learn when a matrix report can be useful and how to create a matrix report in Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
<<<<<<< Updated upstream
last-substantial-update: 2025-05-20T00:00:00.000Z
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
TQID: https://experienceleague.adobe.com/Tk9EtZ83VsH5KaNOfzBuSzx1OJOieeZpewst3OvmtXo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
=======
last-substantial-update: '2025-05-20T00:00:00.000Z'
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
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
=======
autotag-review: '2026-05-06T14:21:46.565Z'
>>>>>>> Stashed changes
---
# Create a matrix report

In this video, you will learn:

* When a matrix report can be useful
* And how to create a matrix report

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on&enablevpops=0)

## Key takeaways

* **Matrix Report Structure:** Matrix reports organize data in rows and columns, with automatic row and column totals. ​ They are ideal for tracking metrics like hours worked, costs, and revenue. ​
* **Filters Setup:** Use filters to focus on specific data, such as hours worked during the last quarter by users from a particular home team. ​ The "owner field source" helps identify relevant team members. ​
* **Grouping Options:** In our example, rows are grouped by "owner name" (person who worked the hours), while columns are grouped by "hour entry date" (by month and week). ​
* **Summarized Data:** Columns like hours, actual cost, and revenue are summarized by default, ensuring totals are displayed in the matrix. These defaults can be turned off, if desired. ​
* **Chart Integration:** Matrix reports can be complemented with charts for alternative data visualization, using the same grouping information. You can set the matrix tab or chart tab as the default view. ​

## "Create a matrix report" activities

### Activity 1: Create a matrix report

Create a matrix report that shows how many requests there are in each status, sorted by request queue. This gives you a quick snapshot of the amount of work coming in and how well you're keeping up with it.

You want the request queues to appear on the row groupings. Status appears as the column groupings. Name your report "Requests by Status and Request Queue."

### Answer 1

1. Select **[!UICONTROL Reports]** from the **[!UICONTROL Main Menu]**.
1. Click the **[!UICONTROL New Report]** option and select **[!UICONTROL Issue]**.
1. Go to the **[!UICONTROL Groupings]** tab and click **[!UICONTROL Switch to Matrix Grouping]**.
1. For [!UICONTROL Row Groupings], select **[!UICONTROL Project]** > **[!UICONTROL Name]**.
1. For [!UICONTROL Column Grouping], select **[!UICONTROL Issue]** > **[!UICONTROL Status]**.

   ![An image of the screen to create a new issue report grouping](assets/matrix-report-groupings.png)

1. Go to the **[!UICONTROL Filters]** tab.
1. To make sure you see only requests in active request queues, add the following filter rules:

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Equal] > [!UICONTROL Current]
   * [!UICONTROL Queue Definition] > [!UICONTROL Is Public] > [!UICONTROL Not Equal] > [!UICONTROL None] (this is how we know a project is actually a request queue, by the Queue Definition being assigned to one of the public options.)

1. Click on **[!UICONTROL Save + Close]**. When prompted for a report name, type in "Requests by Status and Request Queue."

   ![An image of the screen to create a new issue report filter](assets/matrix-report-filters.png)
