---
title: Understand email alerts and proof notifications
description: Understand the difference between email alerts and proof notifications in [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00.000Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
TQID: https://experienceleague.adobe.com/JlKQq4ArHy49-vfGHDRU73cZ0X8RNBlRmb7OEU9xM5A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Understand email alerts and proof notifications

Email alerts are different from proof notification emails. You'll receive a proof notification email when you've been assigned a new proof to review, when a proof is late, or when there's a new version of the proof for you to look at.

![An image of a proof notification email indicating that there is a new proof to review.](assets/email-alert-1.png)

If you turn off the notification option when uploading a proof, then no one receives any communication from [!DNL Workfront] about there being a new proof to review.

Email alerts are set per reviewer/approver, most often as the proof is uploaded. A default email alert type may be assigned to your proof recipients so you don't have to set it each time you upload a proof. Talk to your system administrator about getting these defaults set.

![An image of an email alert indicating that a decision has been made on the proof and there is a comment to review.](assets/email-alert-2.png)

Even if email alerts are set to [!UICONTROL Disabled], proof recipients are still notified of a new proof or version.

## Best Practices

| Best Practice | Here's why |
|---|---|
| Disable the "Send emails from Workfront when a comment is made on a proof" setting in the Workfront setups | When this setting is enabled (which it is by default), users have the potential to get multiple email notifications for each comment on a proof—one from the proofing functionality and one from Workfront itself. These duplicate notifications lead to email notification disruption and confusion, as well as a full email inbox, which may ultimately result in users ignoring proof notifications they receive. Which, in turn, could mean missed deadlines. <br> <br>Note: This setting is found in the Workfront Main Menu > Setup > Email > Review and Approval. |


