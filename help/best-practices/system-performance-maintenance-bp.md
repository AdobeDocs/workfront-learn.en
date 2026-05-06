---
title: Best Practice - System performance and maintenance
description: Explore best practice recommendations from Adobe Workfront experts about Workfront system performance and maintenance.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
TQID: https://experienceleague.adobe.com/2tq7aNHE96fep1EFCPrjcCo13t5lQ24A6c-ORDUmlpY
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
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Best Practice - System performance and maintenance

## What is an Adobe Workfront “best practice”? 

Best practices are guidelines that represent an effective, efficient course of action; are easily adopted by you and the users at your company; and can be replicated successfully across your organization. 

As you review these recommendations, please keep in mind that some Workfront best practices are universal while others might be more specific to the topic. Use these best practices as a framework to help guide your Workfront system setups and use.

## Navigating this page 

As you scroll through this page, first you’ll find a high-level list of all the best practices for the topic. This allows you to review the recommendations without diving into the details of “why.” 

The “Why are these best practices?” area, found after the high-level list, provides greater detail into some of the best practices and why they're deemed as a process, tool, etc., you should consider implementing with your Workfront instance. 

</br>
</br>

## System performance and maintenance best practices 

* Review product release notes before the release date. 

* Create different types of exceptions reports that highlight missing or incorrect data and settings.

* Create a user deactivation process that includes a review of objects that are owned by them or assigned to them so that users who are no longer a part of the company do not remain active in the system and create confusion for other users. 

* Keep workflow configurations as simple as possible to make sure that they are scalable and can be maintained in your absence. 

* Use filters on reports and object lists to decrease the number of rows displayed at one time and focus the team on important information. 

* Regularly clear your browser cache and cookies to help improve performance in Workfront. 

* Start cleaning up your system in major Adobe Workfront areas that tend to be the most cluttered such as custom forms, templates, projects, and users. 

* Know what cluster your Workfront instance is on so you can watch for updates, be aware of maintenance windows, etc. 

* Keep projects short. 

* Where possible, keep reports “light” with very few and uncomplicated filters to improve performance. 

</br>
</br>

## Why are these best practices? 

**Best practice**

Review product release notes before the release date. 



**Here’s why**

The release notes tell you what new functionality and tools are coming to the Workfront system. By reviewing these notes and playing around with the new functionality in the Preview Sandbox environment, you have a chance to learn about, practice with, and resolve any bugs with new enhancements before they’re released to production.

</br>
</br>

**Best practice**

Create different types of exceptions reports that highlight missing or incorrect data and settings.



**Here’s why**

These reports include ones that tell you which users should be deactivated, which projects show completion percentage of 100% but are not marked complete, what templates have never been used, etc. 

 

Put these reports like these, and others, onto a dashboard and give other system and group administrators access to this dashboard to maintain a clean system in a timely manner. For example, the Workfront Cleanup Dashboard and the Workfront Usage Dashboard include report examples you can create. 



To help you remember to check these reports, on at least a quarterly basis, build a project with quarterly tasks and assign them to yourself, and system and group administrators. Make sure these tasks have planned hours associated so assignees of these work items can properly allocate their time. 

</br>
</br>

**Best practice**

Keep projects short.



**Here’s why**

Every time you save a project, or a task inside of the project, there is a timeline calculation running to update all dependencies. Depending on the number of tasks in your project, the recalculation can take a long time to run.
