---
title: Best Practice - Schedules
description: Explore best practice recommendations from Adobe Workfront experts about setting up, managing, and using Workfront schedules.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10925
exl-id: 508d6f90-f9f4-4f12-9bf1-5e89246f3e3a
TQID: https://experienceleague.adobe.com/Lxc0Ymk5tPPsIvM4iKGS68o7eJpFCjgOwWtcQ67aWp4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d3382524-5489-431b-bde9-271ab257bc37
    internal-label: Workfront Scenario Planner
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Best Practice - Schedules

## What is an Adobe Workfront "best practice"? 

Best practices are guidelines that represent an effective, efficient course of action; are easily adopted by you and the users at your company; and can be replicated successfully across your organization. 

As you review these recommendations, please keep in mind that some Workfront best practices are universal while others might be more specific to the topic. Use these best practices as a framework to help guide your Workfront system setups and use.

## Navigating this page 

As you scroll through this page, first you'll find a high-level list of all the best practices for the topic. This allows you to review the recommendations without diving into the details of "why." 

The "Why are these best practices?" area, found after the high-level list, provides greater detail into some of the best practices and why they're deemed as a process, tool, etc., you should consider implementing with your Workfront instance. 

</br>
</br>

## Schedules best practices 

* Limit the number of schedules you create in Adobe Workfront. 

* The total working hours in each working day on the schedule should be equal to the number of hours in a day that is specified in the global project preferences. 

* Add a reminder to the Adobe Workfront system administrator's calendar to update Schedules at a set time each year. 


For instructions on how to create and manage schudules, see the [Create and manage schedules](/help/administration-and-setup/configure-system-defaults/create-and-manage-schedules.md) tutorial.

</br>
</br>

## Why are these best practices? 

**Best practice**

Limit the number of schedules you create in Adobe Workfront. 

  

**Here's why**

Don't create dozens of schedules for different groups, teams, or individuals. Fewer schedules means less maintenance by the system or group administrators. 

 

Separate schedules might be needed when: 

* Employees are in different time zones (U.S. Pacific vs. U.S. Eastern) or different regions (EMEA vs. APAC). 

* You have part-time workers who work less than 40 hours per week. 

* Workers don't work the standard 8 hours a day, Monday-Friday, such as weekend workers or those who work four 10-hour days. 

</br>
</br>

**Best practice** 

The total working hours in each working day on the schedule should be equal to the number of hours in a day that is specified in the global project preferences. 



**Here's why**

If the total working hours don't match, this can result in seemingly incorrect date and time calculations in your project timeline and reports. 

For example, if the system preference is eight hours in a day and the schedule assigned to a project has only seven working hours a day, you'll notice that a task with a one-day duration takes more than one day to complete, because it's trying to fit in the eight hours. 

**Note**: The system global project settings are done in Setup > Project Preferences > Timeline Calculations > Typical hours per work day.

</br>
</br>


**Best practice**

Add a reminder to the Adobe Workfront system administrator's calendar to update Schedules at a set time each year. 

**Here's why**

Update the schedules in your Workfront instance with national holidays, company holidays, and other days users won't be working. Do this at a set time each year, either at the end of the year or when holiday schedules are released by human resources, so project timelines, resource planning, etc., reflect accurate user availability.
