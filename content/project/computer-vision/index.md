---
title: Image Classification
summary: Image recognition of architectural heritage images
tags:
  - Deep Learning
date: '2022-03-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Foto di <a href="https://unsplash.com/it/@mvdheuvel?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Maarten van den Heuvel</a> su <a href="https://unsplash.com/it/foto/0SYJS6nfR10?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
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

In this computer vision project, our goal was to classify architectural heritage images. We had a dataset of 10,235 training images, each sized at 128x128 pixels, and these images fell into 10 different architectural categories.

To build our model, we followed a gradual approach. We began with simple, shallow neural networks and progressively deepened them as we advanced in the model development process. This allowed us to create more complex models over time.

To ensure that our model wouldn't memorize the training data but instead generalize well to new, unseen images, we employed various techniques for regularization. These techniques helped us strike a balance between model complexity and generalization ability.

One of the key strategies we implemented was **data augmentation**. With this technique, we expanded our training dataset by applying transformations to the existing images. Specifically, we used horizontal flipping and random zoom, effectively tripling our training data. This helped our model learn better from a wider variety of examples.

Our model **could correctly classify approximately 8 out of 10 test images**. This demonstrated its capability to accurately identify architectural elements in the images.

Additionally, we assessed our model's performance using the F1 score, which combines precision and recall. 9 out of the 10 architectural categories achieved a good F1 score, surpassing the 0.70 threshold. This indicated that our model excelled in most of categories.

This project was developed on Python via the *Keras* library.

