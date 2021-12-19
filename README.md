## Human-Iris-Center-Detection-ML
This repository contains an implementation for calculating human iris center using CNN model built by PyTorch. The CNN architecture is proposed in [this paper](https://ieeexplore.ieee.org/abstract/document/8803121/), and dataset with face images and labels (iris center coordinates + eye corners) is [here](https://www.unavarra.es/gi4e/databases/gi4e/). It is apart of Assignment2 in Machine Learning course for ROCV master's program at Innopolis University.

---
### Table of Content 
```
├── src              <- directory for source files 
|    ├── main.ipynp  <- contains ipynp notebook
|
├── Task description.pdf       
└── Readme.md
```
---
### Task description
Eyes are considered to be the most salient and stable feature in the computer vision community. Automatic extraction of eyes plays an important role in many real-world applications such as gaze tracking, face alignment, driver drowsiness detection, face recognition, and human–computer interaction, etc. Several factors that make challenging to detect and track eyes are head poses, lighting conditions, shape and color of eyes, iris movement, imagining quality and conditions, etc. A lot of works has been performed to solve the above problems but still, it remains an open area of research in the computer vision community. 
In this task you are going to implement CNN for calculating human iris center. This CNN architecture is proposed in [this paper](https://ieeexplore.ieee.org/abstract/document/8803121/) as a fully convolutional network which consists of a base network and auxiliary network. It has two losses: reconstruction loss for ensuring the model saves important positional features and second loss is the distance between predicted eye center and ground truth one. The architecture also has skip connection which brings position information to deep layer. Dataset with face images and labels (iris center coordinates + eye corners) is [here](https://www.unavarra.es/gi4e/databases/gi4e/). 
You can use cv2 as tool in that task to read, convert color of images, to draw something on image and to do all the other needed operations with images. However, you are not restricted to use it and you can use any libraries. 
