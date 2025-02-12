---
title: Create an automated workflow template
description: Learn how to create an automated workflow template by assigning proof recipients and setting proof deadlines. Then share the template with other users.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
---
# Create an automated workflow template

In this video, you will learn how to:

* Create an automated workflow template for [!DNL  Workfront] proofing
* Assign proof recipients 
* Set a review and approval process deadline
* Share the automated workflow template with others

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops)

## Additional stage activation options

Two options for determining when a proofing workflow stage should kick off are rarely, if ever, used: the [!UICONTROL Date and time] option and the "[!UICONTROL When the previous stage deadline passes]" option.

The second option really only works in scenarios where you have a large group of people reviewing and you don't want to wait on all of them. It's kind of a "I'll give you a certain amount of time to complete your review and then you lose your chance" option. But even this can slow down a review process.

If you do use "[!UICONTROL when the previous stage deadline passes]," it's important to remember that you can manually activate a stage at any time if you don't want to wait for a deadline to pass.

## Best Practices

| Best Practice | Here's why |
|---|---|
| Set the proof creator's proof role to Reviewer. | The Reviewer proof role ensures the proof creator can make comments and access comments left by others. Most of the time, the proof creator isn't required to make a decision on a proof they've uploaded. The Approver, Reviewer & Approver, Author, or Moderator proof roles all require a decision be made. If the proof creator is assigned one of these proof roles but never makes a decision, this can adversely affect proof deadlines. |
|Avoid using the Approver proof role.|The Approver proof role does not allow the user to make comments on this proof. This could lead to a user rejecting the proof, without any explanation because they could not make comments. Use the Reviewer & Approver proof role instead so the user can provide feedback.|
|Avoid the All Activity proof email alert option.|This option sends a proof email notification any time something happens with a proof—a comment is made, a reply is posted, a decision is made, etc. The recipient is essentially seeing proof activity as it happens.<br><br>For proof owners and creators, the Decisions email alert works best for multi-stage proof workflows and Final Decision works best for single-stage workflows. Generally, everyone else can be set to Disabled, unless they want to be notified of other people making comments or decisions (in which case, one of the summary email options might work best).|
