---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
### Biography
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin


### Experience
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Lead Engineer, Machine Learning
          company: Samsung R&D Institute India - Bangalore (SRI-B)
          company_url: ''
          company_logo: '' # org-x # https://images.squarespace-cdn.com/content/v1/619d2006b23f9f7f9f282ea8/2f9744f0-cfc9-435a-82e0-781528a48028/hike_logo.png
          location: India
          date_start: '2023-03-01'
          date_end: ''
          description: |2-
              * Working on identifying bottlenecks and enhancing the Android graphics rendering pipeline by adding improvements in the Android framework
              * Developing an in-house Android profiling tool to benchmark Android rendering uniformly across various Samsung apps and devices

        - title: Senior Software Engineer, Machine Learning
          company: Samsung R&D Institute India - Bangalore (SRI-B)
          company_url: ''
          company_logo: '' # org-x # https://images.squarespace-cdn.com/content/v1/619d2006b23f9f7f9f282ea8/2f9744f0-cfc9-435a-82e0-781528a48028/hike_logo.png
          location: India
          date_start: '2021-03-01'
          date_end: '2023-02-28'
          description: |2-
              * Developed on‐device machine learning (ML) model that uses phone usage data to detect boredom while a user is using their phone
              * Developed an end‐to‐end Android application to demonstrate the effectiveness of the boredom ML model to the stakeholders
              * Worked on developing a deep neural network (DNN) model that uses phone usage data to predict gender and demographic age
              * Developed the above model using TensorFlow Federated and Flower libraries to train it in a Federated Learning (FL) environment
              * Developed a differential privacy-based ML solution for the problem of Privacy Protected Semantic Location Tagging

        - title: Software Engineer, Machine Learning
          company: Samsung R&D Institute India - Bangalore (SRI-B)
          company_url: ''
          company_logo: '' # org-x # https://images.squarespace-cdn.com/content/v1/619d2006b23f9f7f9f282ea8/2f9744f0-cfc9-435a-82e0-781528a48028/hike_logo.png
          location: India
          date_start: '2019-06-20'
          date_end: '2021-02-28'
          description: |2-
              * Developed Android application for visualizing depth maps & 3D Point‐cloud from Time‐of‐Flight (ToF) camera feed in real‐time
              * Developed gesture‐based UI features such as Zoom, Pan, and Rotation for the point‐cloud visualization module in the Android app
              * Worked on developing an on‐device privacy‐preserving DNN model‐based solution for the problem of Next App Recommendation
              * DNN model was designed under strict memory constraints to minimize network bandwidth costs during various FL execution steps
              * Developed and trained the DNN model in Java using the DL4J library so that it can be trained and used on‐device on Android
              * Developed an Android User Trial (UT) application that supported FL, model training, and inference on‐device for the DNN model

        - title: Undergraduate Software Developer Internship
          company: Samsung R&D Institute India - Bangalore (SRI-B)
          company_url: ''
          company_logo: '' # org-x
          location: India
          date_start: '2018-05-13'
          date_end: '2018-07-19'
          description: |2-
              * Developed Neural Network (NN) model to predict the current location of a user based on their recent locations and time of the day
              * Developed a simulation environment for replicating which cell tower in a given area a user would be connected to while in transit
              * Developed an ML classification model to predict which cell tower a user is most likely connected to at any time of the day
              * Top‐1 & Top‐3 prediction accuracies for the final model were 85‐90% and 90‐95% respectively on the evaluation dataset

        - title: Undergraduate Software Developer Internship
          company: Hike Private Limited
          company_url: ''
          company_logo: '' # org-x # https://images.squarespace-cdn.com/content/v1/619d2006b23f9f7f9f282ea8/2f9744f0-cfc9-435a-82e0-781528a48028/hike_logo.png
          location: India
          date_start: '2017-05-13'
          date_end: '2017-07-19'
          # * Developed Image Classifier using Convolutional Neural Network (CNN) to classify images into pre-defined categories
          # * Trained the CNN models using Google ML-Engine APIs
          # * Developed a Server-Client support using Tensorflow Serving
          description: |2-
              * Implemented Convolutional Neural Network (CNN) models using Python and TensorFlow for an image classification problem
              * Used Google ML‐Engine APIs to train various CNN models on the Google Cloud for accelerated experimentations and training
              * Developed Server‐Client support using TensorFlow Serving for exposing REST APIs to generate predictions from the trained models
    design:
      columns: '2'


## Publications
  - block: collection
    id: research
    content:
      title: Research Work
      # text: |-
      #   {{% callout note %}}
      #   Quickly discover relevant content by [filtering publications](./publication/).
      #   {{% /callout %}}
      filters:
        folders:
          - publication   # For some reason, the other directory names are not working properly. Hence kept the dir name as "publication" only
        exclude_featured: false
    design:
      columns: '2'
      view: citation


### Featured Publications
#   - block: collection
#     id: featured
#     content:
#       title: Featured Publications
#       filters:
#         folders:
#           - publication
#         featured_only: true
#     design:
#       columns: '2'
#       view: card


### Projects
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: ML
          tag: Machine Learning
        - name: Robotics
          tag: Robotics
        - name: Parallel Computing
          tag: Parallel Computing
        - name: Other
          tag: Other
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Possible values are: list, compact, card, showcase
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false


### Online Certifications
  - block: accomplishments
    id: online-certifications
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      # title: 'Accomplish&shy;ments'
      title: 'Online Certifications'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        # GAN Specialization
        - certificate_url:     https://www.coursera.org/account/accomplishments/specialization/certificate/5K6ZPFHS438E
          date_end: '2023-12-02'
          date_start: '2023-07-31'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Reinforcement Learning Specialization
          url: 'https://www.coursera.org/specializations/reinforcement-learning'
        # GAN Specialization
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/X3Y95UH88838
          date_end: '2023-05-20'
          date_start: '2023-04-07'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Generative Adversarial Networks (GANs) Specialization
          url: 'https://www.coursera.org/specializations/generative-adversarial-networks-gans'
        # MLOps Specialization
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/ZDZR8C892T9J
          date_end: '2023-03-25'
          date_start: '2022-12-12'
          description: "" #Formulated informed blockchain models, hypotheses, and use cases.
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Machine Learning Engineering for Production (MLOps) Specialization
          url: https://www.coursera.org/specializations/machine-learning-engineering-for-production-mlops
        # Robotics Specialization
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/MDLXE9VZP8L5
          date_end: '2022-09-24'
          date_start: '2021-08-27'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Robotics Specialization
          url: 'https://www.coursera.org/specializations/robotics'
        # CNN
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/NKQNB8H9LQG7
          date_end: '2022-10-30'
          date_start: '2022-10-10'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Convolutional Neural Networks
          url: 'https://www.coursera.org/learn/convolutional-neural-networks'
        # Hyper-parameter tuning
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/487MU4MY73PL
          date_end: '2020-05-23'
          date_start: '2020-05-08'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: 'Improving Deep Neural Networks: Hyperparameter Tuning, Regularization and Optimization'
          url: 'https://www.coursera.org/learn/deep-neural-network'
        # Sequence Models
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/24L8L2MT2FGB
          date_end: '2019-12-02'
          date_start: '2019-11-15'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Sequence Models
          url: 'https://www.coursera.org/learn/nlp-sequence-models'
    design:
      columns: '2'


### Topic Cloud
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'


### Contact
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      # text: |-
      #   Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      # email: azadmrinaal[at]gmail[dot]com
      email: mrinaal[dot]dogra19[at]gmail[dot]com
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      # address:
      #   street: 450 Serra Mall
      #   city: Stanford
      #   region: CA
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        # - icon: twitter
        #   icon_pack: fab
        #   name: DM Me
        #   link: 'https://twitter.com/Twitter'
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
        - icon: linkedin
          icon_pack: fab
          name: DM Me
          link: 'https://www.linkedin.com/in/mrinaald'
      # Automatically link email and phone or display as text?
      autolink: true
      # # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: true
    design:
      columns: '2'


### Skills
#   - block: features
#     content:
#       title: Skills
#       items:
#         - name: Python, JAVA, C/C++, Shell Script (Bash), Golang, LaTeX
#           description: 90%
#           icon: python    # r-project (fab) -> R; chart-line (fas) -> Statistics; camera-retro (fas) -> Photography
#           icon_pack: fab
#         - name: Java
#           description: 100%
#           icon: java
#           icon_pack: fab
#         - name: C++
#           description: 10%
#           icon: cplusplus
#           icon_pack: devicon
#         - name: Shell Script (Bash)
#           description: 10%
#           icon: terminal
#           icon_pack: fas
#         - name: Golang
#           description: 10%
#           icon: camera-retro
#           icon_pack: fas
#         - name: LaTeX
#           description: 10%
#           icon: camera-retro
#           icon_pack: fas


### Recent Posts
  # - block: collection
  #   id: posts
  #   content:
  #     title: Recent Posts
  #     subtitle: ''
  #     text: ''
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       folders:
  #         - post
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: compact
  #     columns: '2'


### Gallery
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'


### Featured Publications
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card


### Recent and Upcoming Talks
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact


### Hero Introduction block
  # - block: hero
  #   content:
  #     title: Hugo Academic Theme
  #     image:
  #       filename: hero-academic.png
  #     cta:
  #       label: '**Get Started**'
  #       url: https://wowchemy.com/templates/
  #     cta_alt:
  #       label: Ask a question
  #       url: https://discord.gg/z8wNYzb
  #     cta_note:
  #       label: >-
  #         <div style="text-shadow: none;"><a class="github-button" href="https://github.com/wowchemy/wowchemy-hugo-themes" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Wowchemy Website Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/wowchemy/starter-hugo-academic" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
  #     text: |-
  #       **Generated by Wowchemy - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

  #       **Easily build anything with blocks - no-code required!**

  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

  #       <!--Custom spacing-->
  #       <div class="mb-3"></div>
  #       <!--GitHub Button JS-->
  #       <script async defer src="https://buttons.github.io/buttons.js"></script>
  #   design:
  #     background:
  #       gradient_end: '#1976d2'
  #       gradient_start: '#004ba0'
  #       text_color_light: true
---
