---
title: Introduction to iterators exercise
description: Learn to use iteration-type apps and perform actions on each bundle of information.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,catalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
    internal-label: Workfront Fusion
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
autotag-review: '2026-05-06T16:42:51.955Z'
---
# Introduction to iterators exercise

Learn to use iteration-type apps and perform actions on each bundle of information.

## Exercise overview

Look at a specific project in Workfront, then look at all the tasks within that project. You will use the increment tool module to count the number of tasks within the project. Finally, you'll use the Set variable module to subtract the Number of Children from the Number of Open Issues to produce a numeric value for each of the task bundles.

   ![Introduction to iterators Image 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Steps to follow

   **Read a project and related tasks.**

1. Start a new scenario. Name it "Introduction to iteration."
1. Choose Workfront as the trigger module, Read a record.
1. For Record Type, choose Project.
1. For Outputs, choose ID, Name, and Description.
1. In the ID field, put the project ID of the Northstar Fashion Exhibitors Booth project from your Workfront test drive instance.
1. Rename this module "Find WF Projects."
1. Add another Workfront module to read the tasks related to this project. Choose the Read Related Records module.
1. For Record Type, choose Project.
1. For the Parent Record ID, choose the ID from the Read a record module.
1. For Collections, select Tasks.
1. For Outputs, select ID, Name, Description, Number of Children, Number of Open Issues, and Work.
1. Rename this module "Read Project's Tasks."
1. Save the scenario, then click Run once to see the outputs.

   + Click on the execution inspector and you see one bundle as input (the project) and 28 bundles as output (the tasks).

   **Count and process iterated bundles.**

1. Add another module after Read Related Records. Choose an Increment function tools module.

   + Leave the Reset a value field as Never and click OK.

1. Rename this module "Count the # of tasks."
1. Add a Set variable module. Set the Variable name to "Random Math."
1. In the Variable value field, subtract the number of open children from the number of open opTasks.

   **It should look like this:**

   ![Introduction to iterators Image 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Rename this module "Random Math."
1. Save the scenario and click Run once.

For each of the tasks produced by the Read Related Records iterator module, Workfront Fusion performed 28 executions. These 28 bundles will continue to be processed throughout the scenario unless an aggregator is added to close the loop.
