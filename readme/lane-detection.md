---
description: >-
  To build a solution for lane detection to stop the vehicle (automated driving)
  when it deviates from the road; 自动驾驶卡车的辅助功能，在某些情况下（比如GPS信号弱）停止测试中的车辆以避免碰撞
cover: >-
  https://images.unsplash.com/photo-1509034466863-08cfa4b776c4?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw3fHxsYW5lfGVufDB8fHx8MTY0OTgxNjY0NQ&ixlib=rb-1.2.1&q=85
coverY: 0
---

# 🚚 Lane Detection

## Solution Design

The idea is to develop a set of programmes to predict the lane and stop the vehicle under certain conditions

![](../.gitbook/assets/image.png)

{% hint style="info" %}
Environment:  Windows platform on testing Trucks; Visual Studio

Language: Python, Notebooks, Html5
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

![](<../.gitbook/assets/image (2).png>)

### 3. Data Process & Calculation&#x20;

* Define key parameters (center of lane, camera angles, thresholds of deviation, position the truck)
* Trigger the signal to stop the vehicles (integration)

![](<../.gitbook/assets/image (3).png>)

### 4. Continous improvement (Model update, reinforcement training etc) &#x20;

## Reference

### 1. Github:

&#x20;     [https://github.com/kevintriwater/LaneDetection\_End2End](https://github.com/kevintriwater/LaneDetection\_End2End)
