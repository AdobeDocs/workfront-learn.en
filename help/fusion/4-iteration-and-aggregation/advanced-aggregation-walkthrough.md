---
title: Advanced aggregation walkthrough
description: Learn how to call a web service to return details about multiple countries and identify population, grouped by sub-region, all in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
<<<<<<< Updated upstream
TQID: https://experienceleague.adobe.com/g1gAk8fTv9rf3etRqJlZrxpOBevN5D0Mg-JFV7wtVgY
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
topic_v2:
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
=======
autotag-review: '2026-05-06T16:33:27.197Z'
>>>>>>> Stashed changes
---
# Advanced aggregation walkthrough

Call a web service to return details about multiple countries and identify the total population of all countries, grouped by sub-region.

![An image of the Fusion scenario](assets/iteration-and-aggregation-3.png)

## Advanced aggregation walkthrough

Workfront recommends watching the exercise walkthrough video before trying to recreate the exercise in your own environment.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## Exercise URLs

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Reinforcement of aggregation principle

Any time a module outputs multiple bundles, every module after that will execute each bundle.

To prevent this, add an aggregator after a module that potentially produces multiple bundles.

You'll see a shadow surrounding any segment in your scenario from a **beginning-iterator** to the **ending-aggregator**. This helps make these segments easy to spot in your Workfront Fusion scenario.

## Your turn

>[!NOTE]
>
>Practice exercises and challenges are optional and are not necessary to complete Fusion training.

This practice exercise builds on what you learned in the walkthrough, but the solution is not provided.

Create a new scenario to sum all hours logged on tasks in projects in the marketing portfolio. Then send one email that says "Your {Project Name} project team has logged {summed hours} of the total {planned hours} planned hours, putting you at {percentage} of the plan."

**Challenge:** See if you can do the same thing but for hours logged this year only.

## Want to learn more? We recommend the following:

[Workfront Fusion documentation](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
