---
title: Detecting Semantically Similar Questions on Quora Dataset
summary: Natural Language Processing Course project
tags:
  - Machine Learning
  - Natural Language Processing (NLP)
date: "2018-04-30T05:30:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: A schematic of the Baseline Architecture with additional LSTM layer
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: 'uploads/nlp_similar_ques_report.pdf'
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

<!-- <h2 >Location</h2> -->
<!-- This project was done as a industrial software internship at Hike Pvt. Ltd., New Delhi, during May ‘17 - Jul ‘17, the summer of my second year. -->
<!-- This project was taken as part of the Robotics club at IIT Kanpur during my first two years at IIT Kanpur. -->


<h2>Details</h2>
<!-- This project was started as part of the course CS657: Information Retrieval, in the Spring ‘18 term at IIT Kanpur under Prof. Arnab Bhattacharya, Department of Computer Science and Engineering, IIT Kanpur. It was later continued beyond the course into my second undergraduate research project. -->
<p style="text-align: justify;">This project was done as part of the course CS671A: Introduction to Natural Language Processing, in the Spring ‘18 term at IIT Kanpur under Prof. Harish Karnick, Department of Computer Science and Engineering, IIT Kanpur.</p>
<!-- This project was done as an undergraduate project, in the Spring ‘18 term at IIT Kanpur under Prof. Indranil Saha, Department of Computer Science and Engineering, IIT Kanpur. -->

<h2>Brief summary of the work done in the project</h2>
<p style="text-align: justify;">Websites like quora provide a platform for Question and Answering across various subjects and fields. However, the websites also contain loads of similar questions which have different sets of replies although they seek same answer. We aim to develop an application which can detect whether two questions on quora are semantically similar. More formally we want a model which when given two questions, gives</p>
<ul>
  <li>0 if both questions cannot be answered by the same answer</li>
  <li>1 if both question can be answered by the same answer</li>
</ul>
<p style="text-align: justify;">depending on whether the questions are similar in terms of meaning or not. The criteria for two questions being semantically similar is that they seek same answer.</p>


<!-- <h3>Attributions:</h3>
<ul>
  <li><a href="https://commons.wikimedia.org/wiki/File:Ada_horizon_green_logo_with_slogan.svg">"Ada programming language logo (2023)"</a> by <a href="https://commons.wikimedia.org/wiki/User:Captain-Haddock17">William J. Franck</a> is licensed under <a href="https://creativecommons.org/publicdomain/zero/1.0/deed.en">CC0 1.0</a> / Merged with other images</li>
</ul> -->