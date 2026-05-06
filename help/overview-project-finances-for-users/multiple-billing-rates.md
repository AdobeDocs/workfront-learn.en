---
title: Understand multiple billing rates
description: Learn how to override system billing rates within a project.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
exl-id: 5b1ae2c4-43bd-4382-900f-078ef84408a5
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
autotag-review: '2026-05-05T19:00:23.025Z'
---
# Understand multiple billing rates

Within [!DNL Workfront], a project manager has the ability to override system billing rates within a specific project. Previously, when the new billing rate was applied to the project, it not only affected future hours but hours already logged on the project.

With [!DNL Workfront]'s new multiple billing rate capability, the project manager is able to decide what period of time a billing rate should be applied. This way, if a rate has been negotiated or changed, the project manager can determine when that rate should take effect.

## Change the billing rate

1. Go to the project's landing page. Select **[!UICONTROL Billing Rates]** from the left panel.

   ![An image of selecting [!UICONTROL Billing Rates] in [!DNL Workfront]](assets/project-finances-1.png)

1. From the **[!UICONTROL Billing Rates]** tab, click the **[!UICONTROL Add Billing Rate]** button. Select **[!UICONTROL New Billing Rate]** from the dropdown.

   ![An image of selecting [!UICONTROL New Billing Rate] in [!DNL Workfront]](assets/project-finances-2.png)

1. The [!UICONTROL New Billing Rate] dialogue box appears. From the **[!UICONTROL Job Role]** dropdown, select the job role to which the new billing rate will be applied.

   ![An image of selecting job roles in a new billing rate in [!DNL Workfront]](assets/project-finances-3.png)

1. Once the job role is selected, the [!UICONTROL Default Billing Rate] and the [!UICONTROL Billing Rate 1] field appear. Enter the new billing rate in the [!UICONTROL Billing Rate 1] field. If that billing rate applies to the whole project (past, present, and future hours logged), click the **[!UICONTROL Save]** button.

   ![An image of saving a new billing rate that applies to the whole project in [!DNL Workfront]](assets/project-finances-5.png)

1. If the new billing rate only applies for a certain period of time, click the **[!UICONTROL Add Rate]** button. The [!UICONTROL Billing Rate 1 End Date] and the [!UICONTROL Billing Rate 2] fields appear. Enter the End Date for [!UICONTROL Billing Rate 1]. You cannot enter a Start Date for [!UICONTROL Billing Rate 1] because the system assumes it started at the beginning of the project.

   ![An image of creating a new billing rate that applies to a certain period of time, starting at the beginning of the project in [!DNL Workfront]](assets/project-finances-6.png)

1. If this is not the case:

   * Enter the default billing rate for [!UICONTROL Billing Rate 1].
   * Select the End Date for [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate]).
   * The Start Date for [!UICONTROL Billing Rate 2] will automatically be set to the day after [!UICONTROL Billing Rate 1] ends.
   * Enter the desired billing rate in the [!UICONTROL Billing Rate 2] section.
   * Continue to add billing rates, as needed, by clicking the **[!UICONTROL Add Rate]** button.
   * When done, click **[!UICONTROL Save]**.
   * All Billing Rates will show in the [!UICONTROL Billing Rates] tab on the project.

   ![An image of creating new billing rates that apply to the different time periods in [!DNL Workfront]](assets/project-finances-7.png)
