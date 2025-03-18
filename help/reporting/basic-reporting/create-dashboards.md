---
title: Create dashboards
description: Organize and display project data with Workfront dashboards, which can be customized, accessed easily, shared, and printed for seamless project management and collaboration.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
exl-id: 7adc2aeb-6618-4894-acc3-298e35175854
doc-type: video
---
# Create dashboards

The video provides a comprehensive guide to understanding and using dashboards in Workfront. 
​It explains that a dashboard is a collection of reports that allows users to organize and display related data in one place. 

>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on)

## Key takeaways

* **Dashboards in Workfront:** A dashboard is a collection of reports that allows users to organize and display related data, such as projects, tasks, and issues, in one centralized view. ​
* **Creating Dashboards:** Dashboards can be customized by selecting a layout, adding reports, custom calendars, or external pages, and arranging them for optimal display. ​ Users can also customize which columns appear in side-by-side reports within the dashboard. ​
* **Accessing Dashboards:** Dashboards can be found under "My Dashboards," "Shared Dashboards," or "All Dashboards" in the Dashboards area. ​ Frequently used dashboards can be pinned or added to favorites for quick access. ​
* **Sharing Dashboards:** Dashboards can be shared with other Workfront users, including all reports within the dashboard, via the "Dashboard Actions" menu. ​
* **Printing Dashboards:** Dashboards can be printed directly from the "Dashboard Actions" menu, making it easy to share physical copies of the data. ​


## "Create dashboard" activities

### Activity 1: Create a dashboard

Create a [!UICONTROL dashboard] with only one report in it—"Search Notes in This Project." This is useful for quickly finding any update made on a project, even if there are thousands of updates to search through. This will search into update threads to quickly extract any updates that meet the criteria you specify in the prompts.

Create this report by making a copy of the "Search Notes" report you created in the "Create a note report" activity (or use another report if you didn't do that activity).

* Remove the Project Name prompt from the copy and rename the report "Search Notes in This Project."
* Name the [!UICONTROL Dashboard] "Search Notes."
* Go to any project landing page and create a custom section for a [!UICONTROL dashboard].
* Note that when you search for notes in your custom section it will only show notes contained within the project you're currently in.

### Answer 1

1. Run the report you created in the "Create a note report" activity. Didn't create it yet? Click here to see the activity in the [Create a task report](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-task-report#activity-1-create-a-note-report-with-prompts) tutorial.
1. Click **[!UICONTROL Report Actions]** and select **[!UICONTROL Copy]**. [!DNL Workfront] creates a new report named "Note Search (Copy)."
1. Go to **[!UICONTROL Report Actions]** and select **[!UICONTROL Edit]**. Click **[!UICONTROL Report Settings]** and change the name to "Search Notes in This Project."
1. Click [!UICONTROL Report Prompts] and delete the [!UICONTROL Project] > [!UICONTROL Name] prompt from the list.

   ![An image of the screen to create a new dashboard](assets/edit-report-prompts.png)

1. Check the **[!UICONTROL Show Prompts in Dashboard]** box.
1. Click **[!UICONTROL Done]**, then **[!UICONTROL Save + Close]**. You now are looking at the [!UICONTROL Prompts] screen of the report.

   Next you're going to use a shortcut to create a new dashboard and add this report to it.

1. Click **[!UICONTROL Report Actions]** and select **[!UICONTROL Add to Dashboard]** > **[!UICONTROL New Dashboard]**.
1. Drag the report "Search Notes in This Project" to the **[!UICONTROL Layout]** panel.
1. Notice that the name of the report becomes the name of the dashboard. Edit the name to just "Search Notes."

   ![An image of the screen to create a new dashboard](assets/create-dashboard.png)

1. Click **[!UICONTROL Save + Close]**.

   Now add the dashboard to a project page.

   ![An image of the screen to create a new dashboard](assets/add-custom-section.png)

1. Go to any project. From the left panel menu, click the **[!UICONTROL Add custom section]** icon.
1. In the **[!UICONTROL Add a Dashboard]** field, type "Search Notes" and select the [!UICONTROL dashboard] from the list.
1. In the **[!UICONTROL Custom section title]** field, type in "Search Notes."
1. Click **[!UICONTROL Add new section]**.
1. From the left panel menu, find Search Notes. Click the dots to the left of the section name and drag it right below Updates.
