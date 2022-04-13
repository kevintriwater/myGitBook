---
description: >-
  To build a solution for lane detection to stop the vehicle (automated driving)
  when it deviates from the road; 自动驾驶卡车的辅助功能，在某些情况下（比如GPS信号弱）停止测试中的车辆以避免碰撞
---

# Lane Detection

## Solution Design

### The idea is to develop a set of programmes to predict the lane and stop the vehicle under certain conditions

![](.gitbook/assets/image.png)

{% hint style="info" %}
Environment:  Windows platform on testing Trucks; Visual Studio

Language: Python, Notebooks, Html5
{% endhint %}

#### 1. Data Collection & Image Process

* Capture the images from Camera on the trucks
* Take x frames per seconds to process at Pixel level

![](<.gitbook/assets/image (1).png>)

#### 2. Predict the lane path

* Find the lane lines (pixels)
* Create a model to predict the path
* Exceptional case handling (light condition ;  weather ; sharp turn)

![](<.gitbook/assets/image (2) (1).png>)

![](<.gitbook/assets/image (2).png>)

#### 3. Data Process & Calculation&#x20;

* Define key parameters (center of lane, camera angles, thresholds of deviation, position the truck)
* Trigger the signal to stop the vehicles (integration)

![](<.gitbook/assets/image (4).png>)

#### 4. Continous improvement (Model update, reinforcement training etc) &#x20;
