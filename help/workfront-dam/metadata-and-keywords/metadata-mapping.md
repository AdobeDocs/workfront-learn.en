---
title: Set up metadata mapping
description: Learn how to set up metadata mapping for [!UICONTROL Workfront DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
TQID: https://experienceleague.adobe.com/MN5oxNgGZsAxmJNwRMRdMfvGnui4m5urnK4q8IdScEM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# Set up metadata mapping

[!DNL Workfront]-related information about an asset can be transferred from [!DNL Workfront] into [!UICONTROL Workfront DAM] with the asset. The metadata mapping option in the [!DNL Workfront] [!UICONTROL Setup] area allows for this transfer of information.

Talk to your [!DNL Workfront] consultant for best practice recommendations on setting up the metadata mapping.

You must be a [!DNL Workfront] administrator and a [!UICONTROL Workfront DAM] administrator to set up metadata mapping. Before you can start, you must connect your [!DNL Workfront] and [!UICONTROL Workfront DAM] accounts.

## Connect accounts

1. Log in to [!DNL Workfront].
1. Open a project, task, or issue and click the **[!UICONTROL Documents]** tab.
1. Click the **[!UICONTROL Add New]** button and select **[!UICONTROL From Workfront DAM]** from the drop-down menu.
1. Enter your login name and password in the [!UICONTROL Workfront DAM] authorization box that appears.
1. Next, click **[!UICONTROL Yes]** to give [!DNL Workfront] access to the [!UICONTROL DAM] account.
1. If needed, refresh the page to update the access to [!UICONTROL Workfront DAM].

With this connection established, now you can start mapping metadata between the two systems. Make sure you've already created the needed metadata fields in [!UICONTROL Workfront DAM] before you start mapping.

## Set up the mapping

1. Log in to [!DNL Workfront].
1. Select **[!UICONTROL Setup]** from the [!UICONTROL Main Menu].
1. Expand the **[!UICONTROL Documents]** section in the left panel menu.
1. Then click on **[!UICONTROL Metadata Mapping]**.
1. In the Workfront field, type the field source of the [!DNL Workfront] field to map.
1. Then select the corresponding or target **[!UICONTROL Workfront DAM]** metadata field.
1. Click the **[!UICONTROL Add Mapping]** button.
1. You'll see the [!UICONTROL Workfront Field Source] and [!UICONTROL Workfront DAM Target Field] in the chart at the bottom of the window.
1. Repeat for all of the desired metadata fields.

![A screenshot of the [!UICONTROL Metadata Mapping] screen in [!DNL Workfront]](assets/01-metadata-mapping.png)
