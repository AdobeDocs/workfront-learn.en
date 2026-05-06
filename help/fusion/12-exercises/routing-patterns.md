---
title: Routing patterns exercise
description: Reinforce your concept of routing and fallback routes without actually dealing with any other APIs.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,catalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
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
autotag-review: '2026-05-06T16:42:16.496Z'
---
# Routing patterns exercise

Reinforce your concept of routing and fallback routes without actually dealing with any other APIs.

## Exercise overview

Use the Set Variable module to send a number through multiple paths to see how filters and fallbacks behave when routing.

   ![Routing patterns Image 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Steps to follow

1. Create a new scenario and call it "Routing patterns and fallbacks".
1. For the trigger, add the Set Variable tool module. Put "My Number" for the Variable name, leave the Variable lifetime as One cycle, and set the Variable field to "75."

   ![Routing patterns Image 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Add another module and choose the Router module. For both paths, choose the Increment function tool and click OK without making any changes for each.

   + For the first path, create a filter, name it "Less than 100," and set the condition to [My Number] Less than 100.

   + For the second path, create a filter, name it "Less than 1000," and set the condition to [My Number] Less than 1000. Make sure you use the Numeric operator for both.

   ![Routing patterns Image 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Routing patterns Image 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Click Run once and watch the bundle pass down the "Less than 100" path.
1. Then change the Set Variable module field to 950 and Run once again. Watch it run down the second path.
1. Click the router and add one more path. Add the Increment function tool module. For the filter, click "The fallback route" checkbox. Notice how the arrow pointing to that path changes to a caret, indicating it's the fallback route.

   ![Routing patterns Image 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Change the Set variable number to 9500 and Run once. Because the number is not less than 100 or less than 1000, the bundle travels down the fallback route.

If you add one more path with an Increment function tool module, but set no filter, what will happen when you click Run once again? Will a bundle ever go down the fallback route with the fourth route added?  

+ No, because with no filter set, every bundle will always go down this path instead of the fallback route.
