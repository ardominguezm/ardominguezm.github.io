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
  - block: resume-biography-3
    content:
      username: admin
      text: |-
        I am a researcher working at the intersection of **Topological Data Analysis (TDA)**,  
        **Ricci curvature**, and **Random Matrix Theory**, with applications in  
        **financial markets**, **EEG & physiology**, and **complex systems**.

        My work focuses on extracting multi-scale geometric and topological signatures from  
        high-dimensional data to improve interpretability, pattern discovery, and modeling  
        of real-world phenomena.  

        I aim to bridge mathematical rigor, computational methods, and data-driven science  
        to understand complexity in finance, neuroscience, and biomedical signals.

      button:
        text: Download CV
        url: uploads/resume.pdf

      headings:
        about: ''
        education: ''
        interests: ''

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
        My research explores the geometry and topology of complex systems through  
        **persistent homology**, **network curvature**, and **spectral analysis**.

        Key domains include:
        - **Financial market dynamics**
        - **Physiological complexity (HRV, EEG)**
        - **Neuroscience & cognitive states**
        - **Fractality & multifractal models**
        - **AI-based classification pipelines grounded in topology and geometry**

        I am always open to collaborations involving complex systems, data-driven modeling,  
        and advanced mathematical tools.

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
