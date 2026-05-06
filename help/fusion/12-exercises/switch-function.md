---
title: Switch function exercise
description: Learn how to use the switch functionality using the Switch function.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
<<<<<<< Updated upstream
TQID: https://experienceleague.adobe.com/qPas3tLs9BC-mSXO3vdMSCz1fxrocAMUOzPI8A3hOGo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
=======
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
    internal-label: Workfront Fusion
>>>>>>> Stashed changes
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
<<<<<<< Updated upstream
=======
autotag-review: '2026-05-06T16:41:24.173Z'
>>>>>>> Stashed changes
---
# Switch function exercise

Learn how to use the switch functionality using the Switch function.

## Exercise overview

For simple data changes, use the Switch function to transform one value to another within a module field. In this exercise, change the two-letter key to the actual name for the project progress status to send in an email.

   ![Switch function Image 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Steps to follow

1. Clone the scenario named "Sharing variables between routing paths."
1. Name the new scenario "Sharing variables between routing paths - Switch."
1. Click the trigger module and add Progress Status to the Outputs section.
1. In the Send an email module, add Progress Status to the Content field.

   + If you just map over the value coming from the Search module, there's a two-letter code for the progress status.
   + To "switch" the code for the full name of each possible progress status, use the "switch" function from the General functions tab.

1. The switch function uses the Progress Status value or expression as a key, then returns the output value based on that key.

   + A key value is defined in the first position after the Progress Status ("LT") with the corresponding output defined in the second position ("Late").
   + The next key value is defined in the third position, with the corresponding output defined in the fourth position, etc., for as many keys as desired.

      ![Switch function Image 2](../12-exercises/assets/switch-function-walkthrough-2.png)
