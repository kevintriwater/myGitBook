---
description: >-
  Using Mathematical Opt and Minimal Cost to reduce inventory investment in
  safety stock on 32K spare parts
cover: >-
  https://images.unsplash.com/photo-1526304640581-d334cdbbf45e?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw5fHxmaW5hbmNpYWx8ZW58MHx8fHwxNjQ5ODIwMzIz&ixlib=rb-1.2.1&q=85
coverY: 0
---

# 💲 Margin Uplift

Minimal Cost Approach to optimize the Safety Stock especially during COVID situation

## Solution Design

### 1. Review current solution

Previous Solution is to use set formula to calculate the Safety Stock over Truck & Bus Parts components

SS (qty) = SS (days) x Past 1 year avg demand, excl. spike outlier month, parts <= 3 order lines in past 12m excluded

SS (days) = 0.8\* x Desirability factor x Risk period x Demand variability

![](<../.gitbook/assets/image (4) (1).png>)

### 2. New model with Mathematical Optimization&#x20;

To develop a new model to forecast the Safety Stock demands

* _<mark style="color:red;">Forecast Error</mark>_ as <mark style="color:blue;">Uncertainty Measure</mark> - forecast errors/ inherent variability as uncertainty measure (than demand)
* _<mark style="color:red;">Demand Segm.</mark>_ <mark style="color:blue;">Cover More Risks</mark> - Groups materials on effectiveness of safety stock measure. Risk protection period -> MRP cycle + lead-time
* _<mark style="color:red;">Minimal Cost Solution</mark>_ - Mathematical model on cost optimization for all w/t given fill rate
* _<mark style="color:red;">Interactive Simulation</mark>_ <mark style="color:blue;">validation</mark> - Consider user defined computational parameters & ensures adherences, as fill rate target, criticality, cost, priority etc.

![](../.gitbook/assets/Picture1.png)

## Reference:

\[1] Sunil Chopra and P Meindl. Supply Chain Management: Strategy, Planning, and Operation. Pearson Education, 6th edition, 2016.&#x20;

\[2] Laurent Lecou e. Internal report: Mftbc after market supply chain man- agement, 2019.&#x20;

\[3] Ivan Pacheco Soto. Classi cation and forecasting for inventory management of spare parts. 11 2015.

\[4] Github:
