---
title: Report on proofs
description: Learn how to use reporting capabilities to manage proof progress.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
TQID: https://experienceleague.adobe.com/hRhnoPYr-S7YWLeHEqq-tieHyBlHkSEkuTtLaYDrpHQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Report on proofs

[!DNL Workfront]'s digital proofing features allow you to manage projects and related review workflows all in one place — [!DNL Workfront]. Gain valuable insight into the proofing work being done with report types, field sources, and field names that display review and approval information.

We recommend working with your [!DNL Workfront] consultant to create reports that meet your organization's requirements. Some of the reports require familiarity with [!DNL Workfront]'s text mode reporting.

Start with these basic, standard reports to help your teams manage proofs going through a review and approval process in [!DNL Workfront].

## [!UICONTROL Proof Approval]

This report type helps you track outstanding proof approvals to make sure deadlines are being met.

![Select [!UICONTROL Proof Approval] from the [!UICONTROL New Report] drop-down menu](assets/proof-system-setups-proof-approval-report.png)

View and filter options include [!UICONTROL decision date], [!UICONTROL proof approval], [!UICONTROL approver stage], [!UICONTROL workflow template], and [!UICONTROL requester information]. With text mode reporting, you can create a grouping that organizes the list by document name. See [Understand basic text mode for groupings](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=en).

When writing proof approval reports, make sure you're getting information related to the most current version of the proofs. [!DNL Workfront] recommends including this field source and field name in the filter:

**[!UICONTROL Proof Approval]>>[!UICONTROL Is Current Document Version]**

![Filters tab in report builder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

This is useful when you're reporting on proofs that have multiple versions so the report lists only the current version of each proof that needs approval. This filters out the earlier versions that you no longer need to work on.

## [!UICONTROL Document Version]

This report type allows you to manage and track versions in [!DNL Workfront].

![Select [!UICONTROL Document Version] from the [!UICONTROL New Report] drop-down menu](assets/proof-system-setups-document-version-report.png)

View options include information from the [!UICONTROL document version], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator], and [!UICONTROL document provider].

Groupings can be done by [!UICONTROL document version], [!UICONTROL entered by], [!UICONTROL proof approval status], or proof owner information.

Filters include [!UICONTROL document version], [!UICONTROL access level], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator], and document provider information.

You can display the name of the proofing stage that is currently active for each document on the report with this column in a view:

**[!UICONTROL Document Versions] >> [!UICONTROL Active Proof Stages]**

![Filters tab in report builder](assets/proof-system-setups-active-proof-stages.png)

If no stage is currently active, the column is blank.

This field source >> field name also is available as a filter in a report.

Use the [!UICONTROL Proof Creator] field source to report on information about the user who created the proof. Choose the [!UICONTROL Name] field source to display the name of the proof creator in a view.

**[!UICONTROL Proof Creator] >> [!UICONTROL Name]**

This field source >> field name combo also is available as a filter.

![Filters tab in report builder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
