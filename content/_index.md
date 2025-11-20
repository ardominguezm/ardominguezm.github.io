---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:

  ##########################################
  # 1) BIO + PHOTO + CV BUTTON (Research focus)
  ##########################################
  - block: resume-biography-2
    content:
      username: admin
      text: |-
        I am driven by a scientific curiosity about how structure and complexity emerge in the world. My research blends ideas from topological data analysis, network geometry, statistical physics, and data science to uncover patterns hidden within high-dimensional data. This exploration has led me across disciplines, from financial markets and physiological signals to human performance, and even to the textures of art, poetry, and collective behavior in computational social science. I enjoy building bridges between mathematical theory and real-world phenomena, using quantitative methods to reveal the shapes, rhythms, and dynamics that govern both human and natural systems.

      button:
        text: Download CV
        url: uploads/resume.pdf

      headings: {}
       
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle

  ##########################################
  # 2) RESEARCH OVERVIEW
  ##########################################
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        My research explores the geometry and topology of complex systems through persistent homology, network curvature, and spectral analysis.

        Key domains include:
        - **Financial market dynamics**
        - **Physiological complexity (HRV, EEG)**
        - **Neuroscience & cognitive states**
        - **Fractality & multifractal models**
        - **AI-based classification pipelines grounded in topology and geometry**

        I am always open to collaborations involving complex systems, data-driven modeling, and advanced mathematical tools.

    design:
      columns: '1'

  ##########################################
  # 3) FEATURED PUBLICATIONS GRID
  ##########################################
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  ##########################################
  # 4) RECENT PUBLICATIONS (citation style)
  ##########################################
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  ##########################################
  # 5) TALKS
  ##########################################
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card

  ##########################################
  # 6) NEWS
  ##########################################
  - block: collection
    id: news
    content:
      title: Recent News
      page_type: blog
      count: 5
      filters:
        exclude_featured: false
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]

---
