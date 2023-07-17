+++

title = "Poker Hands Classifier"
description = "Slides for the project Poker Hands Classifier"
outputs = ["Reveal"]
aliases = [
    "/slides/"
]

+++

# Poker Hands Classifier

---

# Introduction

### Project goal

* Detect and classify poker cards
* Compute the hand score

### Technologies used

* Python 3.10
* Yolo v7
* SSD (later discarded)
* OpenCV
* Jupyter Notebooks

---

# Yolo

YOLO is a popular object detection algorithm that can recognize and localize multiple objects within an image or video in real-time. The YOLO network uses a single convolutional neural network (CNN) architecture to simultaneously perform object detection and classification.

---

# Yolo v7 vs Yolo

* 40% less parameters
* 50% computations performed
* better accuracy
* faster inference speed
* cheaper hardware requirements

---

# Inline images

![Alternative text](https://i.imgur.com/v4AtJry.png)



![](https://i.imgur.com/j1fVZnB.jpg)

---

# Confusion matrix

![](https://i.imgur.com/AFpXWei.png)

---

# Results

![Results](https://i.imgur.com/w3EBRal.png)

---

# Training batch example

![](https://i.imgur.com/mxVRWjS.jpg)

---

# Testing batch example

![](https://i.imgur.com/AKmmO8U.jpg)

---

# Showcase video

<a href="https://youtube.com/shorts/gLaihFNVr9E"><img src="demo.gif"/></a>
