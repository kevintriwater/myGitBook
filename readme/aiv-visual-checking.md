---
description: >-
  Collaboration with ASADE university Data Science Team; In order to turn the
  image captured by AIV camera to meaningful information for stocking,
  differentiation between slots with stocking needs;
cover: >-
  https://images.unsplash.com/photo-1518432031352-d6fc5c10da5a?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHxhdXRvbWF0aW9ufGVufDB8fHx8MTY0OTgyMDQ0Ng&ixlib=rb-1.2.1&q=85
coverY: 0
---

# 🤖 AIV Visual Checking

## Solution Design

The target of the project is to develop and deploy the object detection algorithm which enables the AIVs to conduct automated stock checking of approx. 20-30 shelves in the production area. Although the shelves and part boxes are standardized, there are some constraints that need to be taken into consideration. Namely;

\-Light condition may differ depending on the location of shelves

\-Distance between the camera and shelf may differ depending on the shelf

![](<../.gitbook/assets/image (4).png>)

{% hint style="info" %}
Hardware design of smart shelves

Software design of automated pick-up&#x20;

Identification of bottlenecks for future deployment&#x20;
{% endhint %}

### 1. Data Collection & Image Process

* Capture the images from Camera on the trucks
* Take x frames per seconds to process at Pixel level

![](<../.gitbook/assets/image (1).png>)

### 2. Predict the lane path

* Find the lane lines (pixels)
* Create a model to predict the path
* Exceptional case handling (light condition ;  weather ; sharp turn)

![](../.gitbook/assets/1\_8Ad83Bjglm4UbyekDSpUXw.png)

![](../.gitbook/assets/1\_Jtis7YWHs6FdRtWQrQjA-A.jpeg)

![](../.gitbook/assets/1\_UXc1hiGAOs4t2i1F6iVVMQ.jpeg)

![](<../.gitbook/assets/image (2) (1).png>)

### 3. Data Process & Calculation&#x20;

* Define key parameters (center of lane, camera angles, thresholds of deviation, position the truck)
* Trigger the signal to stop the vehicles (integration)

![](<../.gitbook/assets/image (3).png>)

### 4. Continous improvement

* Model update
* Reinforcement training

## Reference

### 1. Github:

&#x20;     [https://github.com/kevintriwater/LaneDetection\_End2End](https://github.com/kevintriwater/LaneDetection\_End2End)
