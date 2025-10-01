---
title: Multi-task Learning with ToolkenGPT Framework
summary: Developed Neural Network models to learn the physical model of Quadrotor and synthesize its controller
tags:
  - Machine Learning
  - Large Language Models
date: "2024-11-30T05:30:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ToolkenGPT framework from original paper
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: 'https://github.com/mrinaald/ToolkenGPT/tree/cse291a'
url_pdf: 'uploads/cse291a-report.pdf'
url_slides: 'uploads/cse291a-slides.pdf'
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

<!-- <h2 >Details</h2> -->
<p style="text-align: justify;">This project was done as an graduate project, in the Fall '24 term at UC San Diego under Prof. Lian Hui Qin, Department of Computer Science and Engineering, UC San Diego.</p>

<br>

<!-- <h2>Brief summary of the work done in the project</h2> -->
<p style="text-align: justify;">This project explored the capabilities of <b>ToolkenGPT</b>, a modular framework for tool-augmented language models, by integrating it with <b>smaller, modern LLMs</b> like <b>Llama 3.2</b>. My focus was on enabling <b>multi-task learning</b> within this architecture, i.e., training the model to handle diverse tasks like <b>numerical reasoning</b> and <b>knowledge-based QA</b> simultaneously.</p>

<br>

<h2>Project Highlights</h2>
<ol style="text-align: justify;">
  <li> <b>Framework Re-implementation</b>: Adapted ToolkenGPT to work with Hugging Face’s Transformer-based Llama models. This required significant changes to the training, model, and inference pipelines to ensure compatibility and extensibility.
  <li> <b>Multi-task Learning Extension</b>: Designed and implemented a new multitask training pipeline and model (<code>MultiTaskFunctionLM</code>) to support concurrent learning across multiple tasks.
  <li> <b>Experimental Research</b>: Conducted experiments to evaluate task synergy and performance trade-offs in multi-task setups. This included analyzing the effect of joint-task training strategies.
  <li> <b>Evaluation & Benchmarking</b>: Developed custom evaluation scripts for benchmark datasets such as <b>GSM8K</b>, <b>FuncQA</b>, and <b>KAMEL</b>, measuring model generalization and reasoning performance.
</ol>

<br>

<h2>Key Contributions:</h2>
<ol style="text-align: justify;">
  <li> Rewrote core training and inference modules to support Hugging Face models (<code>train_llama.py</code>, <code>inference_llama.py</code>, <code>model.py</code>)
  <li> Introduced a multitask model and training script (<code>multitask_model.py</code>, <code>train_llama_multitask.py</code>)
  <li> Built dataset converters and evaluators for task-specific benchmarks (<code>convert_data.py</code>, <code>eval_gsm8k_funcqa.py</code>, etc.)
</ol>

<br>

<p style="text-align: justify;"><b>Note</b>: The multitask model is still under development and currently supports inference on only the primary task in a multi-task setting due to architectural limitations.</p>

<br>

<h2>Takeaway:</h2>
<p style="text-align: justify;">This project provided hands-on experience in <b>deep model engineering</b>, <b>multi-task learning</b>, and <b>LLM fine-tuning</b>, while demonstrating how tool-augmented models can scale to support flexible reasoning across diverse tasks.</p>


<h3>Attributions:</h3>
<ul style="text-align: justify;">
  <!-- <li><a href="https://commons.wikimedia.org/wiki/File:Ada_horizon_green_logo_with_slogan.svg">"Ada programming language logo (2023)"</a> by <a href="https://commons.wikimedia.org/wiki/User:Captain-Haddock17">William J. Franck</a> is licensed under <a href="https://creativecommons.org/publicdomain/zero/1.0/deed.en">CC0 1.0</a> / Merged with other images</li> -->
  <li>Image source: <a href="https://github.com/Ber666/ToolkenGPT/blob/main/assets/image.png">ToolkenGPT</a> by <i>Hao et al.</i></li>
</ul>
