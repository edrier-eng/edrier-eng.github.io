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
        Materials and devices for solar energy conversion and carbon capture · Department of Chemical Engineering · Ben-Gurion University of the Negev
      primary_action:
        text: Our Research
        url: '/research/'
        icon: hero/beaker
      secondary_action:
        text: Join the Lab
        url: '/opportunities/'
        icon: hero/user-group
      announcement:
        text: "We are hiring PhD students and postdocs!"
        link:
          text: "Apply now"
          url: "/opportunities"
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
        - statistic: "54"
          description: Peer-reviewed publications
          sub_metric: In journals and conference proceedings
          icon: hero/document-text
        - statistic: "8"
          description: Current group members
          sub_metric: MSc, PhD, postdocs & researchers
          icon: hero/user-group
        - statistic: "$5M+"
          description: Competitive research grants
          sub_metric: ISF, BSF, ERC, industry & more
          icon: hero/currency-dollar
        - statistic: "3"
          description: Active research threads
          sub_metric: Energy, materials & electrochemistry
          icon: hero/beaker
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
        url: /#projects
        icon: hero/arrow-right
    design:
      layout: cards
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]

  - block: cta-image-paragraph
    content:
      items:
        - title: 'State-of-the-Art Research Environment'
          text: |
            Our laboratory features cutting-edge equipment and modern research facilities designed to support breakthrough discoveries. From advanced computational clusters to precision instrumentation, we provide our researchers with the tools they need to push the boundaries of science.
          image: pexels-polina-tankilevitch-3735769.jpg
          feature_icon: hero/check-circle
          features:
            - 'High-Performance Computing: 500+ core GPU cluster for AI/ML research'
            - 'Advanced Instrumentation: Precision equipment for materials characterization'
            - 'Safety & Compliance: Full safety protocols and regulatory compliance'
          button:
            text: 'Virtual Lab Tour'
            url: '/facilities'

        - title: 'Collaborative Innovation Culture' 
          text: |
            Breakthrough research happens through collaboration. Our open lab environment fosters cross-disciplinary partnerships, knowledge sharing, and mentorship between senior researchers and emerging scientists. Every team member contributes to our collective mission of advancing scientific understanding.
          image: pexels-canvastudio-3153198.jpg
          feature_icon: hero/users
          features:
            - 'Cross-Disciplinary Teams: Biologists, engineers, and computer scientists working together'
            - 'Knowledge Sharing: Weekly seminars and collaborative research meetings'
            - 'Mentorship Program: Structured guidance for PhD students and postdocs'
          button:
            text: 'Join Our Community'
            url: '/opportunities'
    design:
      css_class: "bg-white dark:bg-gray-800"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: team-showcase
    id: team
    content:
      title: Meet Our Team
      subtitle: 'World-class researchers pushing the boundaries of science'
      text: 'Our diverse team of researchers brings together expertise from multiple disciplines to tackle the most challenging problems in computational biology and machine learning.'
      user_groups:
        - Principal Investigators
        - Postdoctoral Researchers
        - PhD Students
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
    id: projects
    content:
      title: Active Research Projects
      subtitle: ''
      text: ''
      filters:
        folders:
          - projects
      count: 0  # Number of items to show (0 = all)
      # Default filter UI (for future release)
      #default_button_index: 0
      # Filter toolbar (optional)
      # Add or remove as many filters as you like
    #   buttons:
    #     - name: All
    #       tag: '*'
    #     - name: Machine Learning
    #       tag: ML
    #     - name: Biology
    #       tag: Biology
    #     - name: Materials
    #       tag: Materials
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
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
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: events
    content:
      title: Events
      subtitle: Join Us for Research Presentations & Seminars
      text: Stay connected with our research community through talks, workshops, and collaborative events
      filters:
        folders:
          - events
        exclude_past: false  # Show both past and future events
      count: 3
      sort_by: Date
      sort_ascending: false
    design:
      view: card
      # columns: 3
      show_date: true
      show_read_time: false
      show_read_more: true
      css_class: "bg-gradient-to-b from-white to-gray-50 dark:from-gray-800 dark:to-gray-900"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: collection
    id: news
    content:
      title: Lab News & Updates
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      columns: 1

  - block: logos
    content:
      title: Collaborators & Partners
      subtitle: Leading the way together
      text: We work with top universities, research institutes, and industry leaders to advance scientific discovery
      logos:
        - name: MIT
          image: partners/placeholder-logo.svg
          url: https://mit.edu
          external: true
          description: Massachusetts Institute of Technology
        - name: Stanford University
          image: partners/placeholder-logo.svg
          url: https://stanford.edu
          external: true
          description: Stanford Research Collaboration
        - name: Google Research
          image: partners/placeholder-logo.svg
          url: https://research.google
          external: true
          description: AI & Machine Learning Partnership
        - name: National Science Foundation
          image: partners/placeholder-logo.svg
          url: https://nsf.gov
          external: true
          description: Research Funding Partner
        - name: Microsoft Research
          image: partners/placeholder-logo.svg
          url: https://www.microsoft.com/research
          external: true
          description: Computing Research Collaboration
        - name: NIH
          image: partners/placeholder-logo.svg
          url: https://nih.gov
          external: true
          description: National Institutes of Health
      cta:
        text: Become a Partner
        url: /#contact
        icon: hero/user-plus
    design:
      display_mode: grid
      show_pattern: false
      css_class: "bg-gradient-to-b from-white to-gray-50 dark:from-gray-800 dark:to-gray-900"
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: contact-info
    id: contact
    content:
      title: Contact Us
      subtitle: "Currently on sabbatical at IREC Barcelona (2025–2026). Email is the best way to reach us."
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
        text: Interested in joining our lab? We are always looking for motivated researchers at all levels.
        button:
          text: View Open Positions
          url: /opportunities
      map_url: https://maps.google.com/?q=Ben-Gurion+University+of+the+Negev,+Be'er+Sheva,+Israel
      show_form: false
    design:
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]

  - block: cta-card
    content:
      title: Join Our Research Team
      text: We are always looking for talented and motivated researchers to join our lab. We have openings for PhD students, postdoctoral researchers, and research scientists.
      button:
        text: View Open Positions
        url: /opportunities
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---