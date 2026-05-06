---
title: Filters exercise
description: Learn how to use the filter between modules to allow only certain types of bundles through.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
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
autotag-review: '2026-05-06T16:43:22.961Z'
---
# Filters exercise

Learn how to use the filter between modules to allow only certain types of bundles through.

## Exercise overview

Add a filter between the two modules in the Beyond basic mapping scenario to only create projects that have a "Red" project color in the CSV file.

   ![Filters Image 1](../12-exercises/assets/filters-walkthrough-1.png)

## Steps to follow

1. Create a clone of the "Beyond basic mapping" scenario and name it "Using the mighty filter."

    **Add a filter before the Create Workfront projects module to only allow red projects to be created.**

   ![Filters Image 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Add a filter by clicking the dotted line connecting the modules or clicking the wrench and selecting Set up a filter.
1. Use the Label field to name the filter "Only Red Projects."
1. In the Condition field, map the Project Color field (Column 3 in the CSV file). Select the Equal to (case insensitive) operator, and then type in "red."
1. Click OK.

   ![Filters Image 3](../12-exercises/assets/filters-walkthrough-3.png)

    **Test the filter and verify the results.**

1. Click Save to save the scenario and then Run once.
1. Click the execution inspector for the filter to see how each bundle was examined by the filter and either passed or failed to move on to the Create Workfront projects module.

   ![Filters Image 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Find the projects created in your Workfront instance.
