---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: hero
    id: about
    content:
      title: |
        **Edri Lab**
      text: |
        Materials and devices for solar energy conversion, carbon capture, and utilization.

        Department of Chemical Engineering · Ben-Gurion University of the Negev
      primary_action:
        text: Our Research
        url: '/research/'
        icon: hero/beaker
      secondary_action:
        text: Join the Lab
        url: '/opportunities/'
        icon: hero/user-group
    design:
      # For full-screen, add `min-h-screen` below
      css_class: ""
      background:
        # Option A: Modern gradient mesh (recommended for 2025/2026)
        gradient_mesh:
          enable: true
          style: "waves"
          animation: "pulse"
          intensity: "medium"
          colors:
            - "primary-500/30"
            - "blue-600/20"
            - "indigo-600/15"
        
        # Option B: Team/lab image (uncomment to use instead of gradient mesh)
        # image:
        #   filename: "team-lab-hero.jpg"
        #   filters:
        #     brightness: 0.6
        #     contrast: 1.1

  - block: stats
    content:
      items:
        - statistic: "10"
          description: Active members
          sub_metric: Students & researchers, all levels
          icon: hero/user-group
        - statistic: "20"
          description: Alumni
          sub_metric: Including 2 high-school researchers
          icon: hero/academic-cap
        - statistic: "100%"
          description: Proud of our people
          sub_metric: Every level, every project
          icon: hero/heart
    design:
      layout: cards
      # Section background color (CSS class)
      css_class: "bg-gradient-to-b from-primary-50 to-white dark:from-primary-900/20 dark:to-gray-800"
      spacing:
        padding: ["3rem", 0, "3rem", 0]

  - block: research-areas
    content:
      title: Research Focus Areas
      subtitle: Energy, Materials & Electrochemistry
      text: We combine materials synthesis, thin-film fabrication, and electrochemical methods to develop semiconductor devices for solar energy conversion and CO₂ utilization
      items:
        - name: CO₂ Electroreduction
          description: Designing electrode materials, interfaces, and electrochemical processes that convert CO₂ into useful fuels and chemicals using renewable electricity
          icon: hero/beaker
          gradient: from-green-400 to-teal-600
          status: active
          topics:
            - Electrode Materials
            - Electrocatalysis
            - CO₂ Utilization
            - Carbon Capture
            - Electrolyzers
          cta:
            text: Explore Projects
            url: /research/co2-electroreduction

        - name: PV & Self-Healing Semiconductors
          description: Investigating quasi-1D and layered semiconductor materials with intrinsic self-healing properties for SWIR solar cells and next-generation photovoltaics
          icon: emoji/sun
          gradient: from-yellow-400 to-orange-500
          status: active
          topics:
            - Quasi-1D Materials
            - SWIR Solar Cells
            - Self-Healing
            - Thin Films
            - Defect Chemistry
          cta:
            text: View Research
            url: /research/pv-self-healing

        - name: Photoelectrochemistry & Carbon Capture
          description: Using illuminated perovskite and silicon photoelectrodes to capture CO₂ with sunlight — lowering the energy cost of carbon capture
          icon: emoji/atom_symbol
          gradient: from-blue-400 to-indigo-600
          status: active
          topics:
            - Perovskite Photoelectrodes
            - Light-Driven CO₂ Capture
            - Photoelectrochemistry
            - Interface Engineering
            - Carbon Capture
          cta:
            text: Learn More
            url: /research/photoelectrochemistry
      cta:
        text: Active Research Projects
        url: /research/
        icon: hero/arrow-right
    design:
      layout: cards
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]

  - block: cta-image-paragraph
    content:
      items:
        - title: 'Graduate Training & Research'
          text: |
            Students here take ownership of a real research question from day one — a CO₂-to-formate gas-diffusion electrode, a self-healing antimony-selenide absorber, a CO₂-capturing electrocatalytic membrane — and build the electrochemistry, thin-film growth, and microscopy skills to answer it. Several have co-authored papers before finishing their degree, and former members have gone on to postdoctoral positions and, in some cases, faculty roles.
          image: graduate-training.jpg
          button:
            text: 'See Open Positions'
            url: '/opportunities/'

        - title: 'A Collaborative Research Environment'
          text: |
            Our 120 m² lab carries an idea from synthesis to working device under one roof: atomic-layer and thermal deposition, CO₂ electrolyzers, a multi-channel potentiostat bench, deep-level transient spectroscopy, and an FTIR spectrometer configured for in-situ electrochemistry — complemented by access to BGU's IKI Center for XPS and electron microscopy.
          image: collaborative-research.jpg
          button:
            text: 'Explore Our Facilities'
            url: '/facilities/'
    design:
      css_class: "bg-white dark:bg-gray-800"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: collection
    id: publications
    content:
      title: Selected Publications
      text: ''
      filters:
        folders:
          - publication
        featured_only: true
      count: 5
    design:
      view: citation

  - block: markdown
    content:
      title: Our Funders
      text: |
        We gratefully acknowledge research funding from the [Israel Science Foundation (ISF)](https://www.isf.org.il), [Israel Ministry of Energy](https://www.gov.il/en/departments/ministry_of_energy), [Israel Innovation Authority](https://innovationisrael.org.il/en/), [Israel National Institute for Energy Storage (INES)](https://ines.org.il), and the National Solar Energy Conversion Research Center.
    design:
      css_class: "bg-gradient-to-b from-white to-gray-50 dark:from-gray-800 dark:to-gray-900 text-center"
      spacing:
        padding: ["4rem", 0, "4rem", 0]
---