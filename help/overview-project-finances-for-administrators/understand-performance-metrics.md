---
title: Understand performance metrics
description: Learn how to use the performance metrics - the [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) and the [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
hide: true
exl-id: a7dbd937-0caa-4eb6-bb5d-bff6705e2972
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
autotag-review: '2026-05-05T19:02:44.647Z'
---
# Understand performance metrics

Two performance metrics used by project managers include the [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) and the [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]). System-wide defaults can be set in [!DNL Workfront] and apply to newly created projects. [!UICONTROL PIM] can then be modified on individual projects.

**[!UICONTROL PIM]**

The settings for the [!UICONTROL PIM] control how [!DNL Workfront] calculates other project performance metrics such as the [!UICONTROL Cost Performance Index] ([!UICONTROL CPI]), [!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI]), [!UICONTROL Schedule Performance Index] ([!UICONTROL SPI]), and [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).

Options for the [!UICONTROL PIM] are hour-based and cost-based.

* **Hour-based** — Workfront uses the planned hours in calculating the CPI and EAC of the project. The EAC of the project displays as a number, in hours.
* **Cost-based** — Workfront uses the planned labor cost in calculating the CPI and EAC of the project. EAC appears as a currency value. When using this option, ensure task assignees (users and/or job roles) are associated with cost rates.

**[!UICONTROL EAC]**

[!UICONTROL EAC] represents the projected total cost of your task or project when it completes. Options are calculated at a project level and roll up from tasks/subtasks.

* **Calculate at project level** — [!UICONTROL EAC] for the parent task and project are determined using the actual hours/actual labor costs in [!UICONTROL EAC] formulas. The calculation includes actual hours/costs and expenses added directly to the parent task or project.
* R**oll up from tasks/subtasks** — [!UICONTROL EAC] for the parent task and project are determined by adding up the [!UICONTROL EAC] for each child task. This calculation excludes actual hours/costs added directly to a parent task or project.

The [!UICONTROL EAC] calculations are listed in [Calculate Estimate At Completion (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Performance Metrics: Settings**

To set [!UICONTROL PIM] and [!UICONTROL EAC] system defaults:

1. Select **[!UICONTROL Setup]** from the main menu.
1. Click **[!UICONTROL Project Preferences]** in the left panel menu, then click **[!UICONTROL Projects]**
1. In the [!UICONTROL Project Status] section, find [!UICONTROL Performance Index Method]. Select Hours-based or Cost-based.
1. For [!UICONTROL Estimate at Completion], select Calculate at project level or Roll up from tasks/subtasks.
1. Click **[!UICONTROL Save]** at the bottom of the window.

![An image of the [!UICONTROL Project Preferences] screen](assets/setting-up-finances-1.png)

**Set [!UICONTROL PIM] on individual projects**

1. Go to the landing page of a project.
1. Click **[!UICONTROL Project Details]** from the left panel.
1. Open the **[!UICONTROL Finance]** section.
1. Double-click the text below **[!UICONTROL Performance Index Method]** to edit it.
1. Select Hours-based or Cost-based. 
1. Click **[!UICONTROL Save]** Changes to finish.

![An image of the [!UICONTROL Project Details] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] can be set on a project template, in the [!UICONTROL Finance] section of the template details.
