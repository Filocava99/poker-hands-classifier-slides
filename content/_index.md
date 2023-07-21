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

# Dataset 1/3

* 20.000 immagini
* 416 x 416 pixel
* Etichette formato Yolo v5
* Suddivisione dei set
  * 70% training set
  * 20% validation set
  * 10% test set

---

# Dataset 2/3

* Generazione del dataset:
  * segmentazione
    * conversione in colori binari (bianco/nero) (threshold ~rgb(0,0,0))
    * apertura => chiusura
    * applicazione della maschera sull'immagine originale per ritagliare i pixel della carta
  * ridimensionamento casuale
  * applicazione di un background casuale ottenuto dal [dataset DTD](https://www.robots.ox.ac.uk/~vgg/data/dtd/)

---

# Dataset 3/3

<table>
    <tr>
        <td>
            <image src="https://i.imgur.com/j1fVZnB.jpg" width=¨50¨ max-h="50"/>
        </td>
        <td>
            <image src="https://i.imgur.com/v4AtJry.png" width=¨50¨ max-h="50"/>
        </td>
    </tr>
</table>

---

# Confusion matrix

![](https://i.imgur.com/AFpXWei.png)

---

# Results

![Results](https://i.imgur.com/w3EBRal.png)

---

# Possible future improvements

* Data augmentantion
  * distortion
  * enlargement
  * noise
* in-game suggestions

---

# Training batch example

![](https://i.imgur.com/mxVRWjS.jpg)

---

# Testing batch example

![](https://i.imgur.com/AKmmO8U.jpg)

---

# Showcase video

<a href="https://youtube.com/shorts/gLaihFNVr9E"><img src="demo.gif"/></a>
