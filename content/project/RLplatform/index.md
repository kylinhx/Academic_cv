---
title: Reinforcement Learning Platform of King of FightXV
summary: In our project, we leverage the YOLOv8 model for both character pose recognition and localization. We employ various digital image processing algorithms to extract relevant information from the game screen. Additionally, we utilize the Gym library to construct an environment that facilitates real-time interaction between the environment and an intelligent agent powered by reinforcement learning algorithms.
tags:
  - Others
date: '2023-9-1'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by Xu Han
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
We captured in-game images and meticulously annotated approximately 1000 pictures using the Labelme tool, annotating both positional information and task-oriented actions. This dataset was subsequently partitioned into training, validation, and test sets in an 8:1:1 ratio. Leveraging the YOLOv8 pre-trained model, our training process spanned 150 epochs, resulting in an impressive 99% accuracy on the test set. The computational power for this endeavor came from an Intel Core i7 12700F processor paired with an NVIDIA RTX 3060ti graphics card, which proved instrumental in both the training and testing phases.

![result](result.png)

We implemented a custom environment class using the OpenAI Gym library, where we not only rewrote relevant functions but also introduced additional features such as image information extraction. The environment offers a rich set of interfaces for easy integration and customization. Users can effortlessly tailor the functionality to their specific needs by modifying the relevant Python files.

While we've pre-defined actions for the agent, it's worth noting that in the context of the King of Fighters (KOF) game, our defined moves may not encompass all possible actions. This observation emphasizes the dynamic and diverse nature of in-game scenarios, prompting us to acknowledge the need for ongoing refinement and expansion of the predefined agent actions to ensure a more comprehensive and adaptable reinforcement learning framework.

![val](val.png)



At present, our system supports agent control of Kyo Kusanagi, engaging in battles against the computer-controlled Iori Yagami. Looking ahead, our aspiration is to extend the capabilities to facilitate scenes where two agents engage in combat. The realization of dual-agent battles may necessitate enhanced computational resources, potentially requiring more advanced graphics cards for optimal performance and efficiency. This expansion is anticipated to bring about more complex and nuanced interactions within the King of Fighters game environment.