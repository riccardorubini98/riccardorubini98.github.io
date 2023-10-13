---
title: Reviews analysis and processing
summary: Sentiment analysis and topic modelling of Amazon e-books reviews
tags:
  - Machine Learning
date: '2022-02-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Foto di <a href="https://unsplash.com/it/@like_that_mike?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Mike Kienle</a> su <a href="https://unsplash.com/it/foto/v7KWJRqPncQ?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
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

In this project, we conducted two common tasks in text mining using a large collection of e-book reviews from Amazon.com. Our main objectives were as follows:

**Text Classification for Sentiment Analysis:** Our first goal was to automatically determine the sentiment expressed in the reviews, whether they were positive or negative. To accomplish this, we employed a supervised technique known as Text Classification. After experimenting with various methods, we found that the lasso logistic classifier provided the most satisfactory results. It achieved a recall rate of 92% for positive reviews and 90% for negative reviews. In simpler terms, this means that our model was able to accurately identify whether a review was positive or negative in the majority of cases.

**Topic Modeling:** The second objective of our project was to uncover the main topics discussed in the e-book reviews. We used an unsupervised technique called Topic Modeling for this purpose. Imagine it as a method to identify the key themes or subjects that frequently came up in the reviews. After trying different approaches, we discovered that the algebraic Non-negative Matrix Factorization (NMF) technique was the most effective in identifying reliable topics. These topics were related to various aspects, such as different shades of opinions and various categories of books that were being reviewed.

In summary, our project involved analyzing a large number of e-book reviews from Amazon.com. We used machine learning techniques to determine whether the reviews were positive or negative (sentiment analysis) and to identify the main topics that emerged from these reviews (topic modeling). The results of our efforts showed that our models were quite accurate in sentiment analysis, and we were able to extract meaningful topics from the reviews using advanced mathematical techniques like NMF.

