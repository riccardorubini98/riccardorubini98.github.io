---
title: MSc Thesis - PROMET
summary: An adaptive prompt-based approach for Fine-grained Entity Typing
tags:
  - Deep Learning
date: '2023-05-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  
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

In my thesis, I focused on addressing the Fine-grained Entity Typing task (FET), specifically in few-shot scenario, where only a limited amount of annotated data is available for training. In recent years, there has been a significant advancement in using prompt-based approaches for FET, leveraging Pre-trained Language Models (PLMs) MLM capabilities. These approaches, particularly in few-shot scenarios, have demonstrated superior performance by transforming the entity classification task into a *cloze*-style task based on masked tokens.

However, these existing methods have encountered challenges, primarily related to the requirement of defining specific keywords for each label in the classification set. In my research, I introduced a novel approach called PROMET (PROmpt-tuning using implicit Mask filling for Entity Typing) to overcome these issues. PROMET utilizes the information extracted from the *cloze*-style task by directly leveraging the masked token embeddings, eliminating the need to pass through the masked language modeling head of the PLM. This innovation enables PROMET to operate without the keyword search and reduces its parameter count significantly, making it more efficient compared to other prompt-based methods.

Furthermore, I developed two distinct implementation modes for PROMET: one referred to as *flat*, which consists of a single model, and another called *stack*, involving a hierarchical system of classifiers. The stack mode takes into account the inherent hierarchy among labels in the classification set.

Benchmark results from my research demonstrated that PROMET in the flat mode achieves performance that aligns with the current state of the art, despite its simplicity compared to other approaches. PROMET in flat mode outperforms the stack mode. However, the latter is characterized by greater flexibility and modularity, aspects that make it preferable in the ontology specialization scenario.

In summary, my thesis project introduced PROMET, a novel prompt-based approach for the Fine-grained Entity Typing task, which addresses the challenges of few-shot learning while maintaining competitive performance and offering flexibility through different implementation modes.

Full Thesis can be accessed at this [link](https://drive.google.com/file/d/1vL1OhKphkRIpsDQQDmomHL6mC9CExk-W/view?usp=sharing)

