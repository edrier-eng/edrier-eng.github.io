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
          description: Engineering perovskite-based photoelectrodes that harvest sunlight to drive CO₂ reduction and water splitting, bridging photovoltaics with solar fuels
          icon: emoji/atom_symbol
          gradient: from-blue-400 to-indigo-600
          status: active
          topics:
            - Perovskite Photoelectrodes
            - Solar Fuels
            - Water Splitting
            - Light-Driven CO₂ Reduction
            - Interface Engineering
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
        - title: 'A Collaborative Research Environment'
          text: |
            Our lab combines materials chemistry, electrochemistry, and device physics in a single 120 m² facility at BGU. From ALD and thermal evaporation to CO₂ electrolyzers and FTIR spectroscopy, researchers have direct in-house access to the tools they need, complemented by priority access to the IKI Center for Nanoscience and Nanotechnology at BGU.
          image: pexels-polina-tankilevitch-3735769.jpg
          button:
            text: 'Explore Our Facilities'
            url: '/facilities/'

        - title: 'Graduate Training & Research'
          text: |
            Group members work on open questions in solar energy conversion and CO₂ utilization — from self-healing semiconductors to electrocatalytic membranes. Alumni have continued to postdoctoral, faculty, and industry positions worldwide.
          image: pexels-canvastudio-3153198.jpg
          button:
            text: 'See Open Positions'
            url: '/opportunities/'
    design:
      css_class: "bg-white dark:bg-gray-800"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: team-showcase
    id: team
    content:
      title: Meet Our Team
      subtitle: ''
      text: 'Our group brings together students and researchers with backgrounds in chemical engineering, chemistry, physics, and materials science.'
      user_groups:
        - Principal Investigators
        - Postdoctoral Researchers
        - Research Associates
        - PhD Students
        - MSc Students
        - Undergraduate Students
      sort_by: 'Params.last_name'
      sort_ascending: true
      cta:
        text: View All Team Members
        url: /authors
        icon: user-group
    design:
      show_role: true
      show_organizations: false
      show_interests: true
      show_social: true
      # Section background color
      css_class: "bg-gray-50 dark:bg-gray-900"
      # Reduce spacing
      spacing:
        padding: ["3rem", 0, "3rem", 0]

  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
      count: 5
    design:
      view: citation

  - block: collection
    id: featured
    content:
      title: Featured Research
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: news
    content:
      title: Lab News
      page_type: blog
      count: 3
      filters:
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      order: desc
    design:
      view: card
      columns: 1

  - block: markdown
    content:
      title: Our Funders
      text: |
        We gratefully acknowledge research funding from the [Israel Science Foundation (ISF)](https://www.isf.org.il), [Israel Ministry of Energy](https://www.gov.il/en/departments/ministry_of_energy), [Israel Innovation Authority](https://innovationisrael.org.il/en/), [Israel National Institute for Energy Storage (INES)](https://ines.org.il), the National Solar Energy Conversion Research Center, and the [Blechner Center for Industrial Catalysis and Process Development](https://in.bgu.ac.il/blechner) at BGU.
    design:
      css_class: "bg-gradient-to-b from-white to-gray-50 dark:from-gray-800 dark:to-gray-900 text-center"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: contact-info
    id: contact
    content:
      title: Contact Us
      subtitle: "Email is the best way to reach us."
      visit_title: Visit Our Lab
      connect_title: Connect With Us
      address:
        lines:
          - Department of Chemical Engineering
          - Ben-Gurion University of the Negev
          - 1 Ben-Gurion Blvd.
          - Be'er Sheva 8410501
          - Israel
      office_hours:
        - "By appointment"
      email: edrier@bgu.ac.il
      social:
        - icon: brands/linkedin
          url: https://www.linkedin.com/in/eran-edri-8988b64/
      prospective:
        title: Prospective Members
        text: We welcome inquiries from prospective PhD students, and from BGU Chemical Engineering undergraduates interested in research.
        button:
          text: View Open Positions
          url: /opportunities
      map_url: https://maps.google.com/?q=Ben-Gurion+University+of+the+Negev,+Be'er+Sheva,+Israel
      show_form: false
    design:
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]
---