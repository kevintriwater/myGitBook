---
description: >-
  Using Mathematical Opt and Minimal Cost to reduce inventory investment in
  safety stock on 32K spare parts
---

# Safety Stock Optimization

Minimal Cost Approach to optimize the Safety Stock especially during COVID situation

#### 1. Previous Solution is to use set formula to calculate the Safety Stock over Truck & Bus Parts components

SS (qty) = SS (days) x Past 1 year avg demand, excl. spike outlier month, parts <= 3 order lines in past 12m excluded

SS (days) = 0.8\* x Desirability factor x Risk period x Demand variability

#### 2. Create a model with Mathematical Optimization to forecase the Safety Stock demands

* _<mark style="color:red;">Forecast Error</mark>_ as <mark style="color:blue;">Uncertainty Measure</mark> - forecast errors/ inherent variability as uncertainty measure (than demand)
* _<mark style="color:red;">Demand Segm.</mark>_ <mark style="color:blue;">Cover More Risks</mark> - Groups materials on effectiveness of safety stock measure. Risk protection period -> MRP cycle + lead-time
* _<mark style="color:red;">Minimal Cost Solution</mark>_ - Mathematical model on cost optimization for all w/t given fill rate
* _<mark style="color:red;">Interactive Simulation</mark>_ <mark style="color:blue;">validation</mark> - Consider user defined computational parameters & ensures adherences, as fill rate target, criticality, cost, priority etc.

![](.gitbook/assets/Picture1.png)
