---
title: Detection Box - Assisting Night Driving with Infrared Camera
summary: This is a small box that uses the YOLO model to perform real-time detection of pedestrians, vehicles, and other objects in front of the vehicle, especially in low visibility conditions such as nighttime or heavy fog. It assists drivers by displaying the results using HUD (a display technology). The box achieves a speed of over 150 frames per second and maintains an accuracy rate of over 50%.
tags:
  - Deep Learning
date: '2023-11-14'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by Xu Han on iPhone
#   focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Compared to traditional threshold segmentation algorithms, deep learning-based object detection methods exhibit higher accuracy and stronger robustness. In infrared image object detection tasks, threshold segmentation algorithms are susceptible to various factors, such as the types of clothing pedestrians wear (more clothing leads to decreased recognition performance in cold weather). In contrast, algorithms based on the YOLO model are more comprehensive. They have matured to effectively address these complex scenarios, not only improving the accuracy of object detection but also enhancing the system's adaptability to diverse environmental changes.

![example_inf](example_inf.png)


We tested our device on real roads, and the performance of our recognition model and device is quite impressive. Here are some results from the tests we conducted on roads near our company.