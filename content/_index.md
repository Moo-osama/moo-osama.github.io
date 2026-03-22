---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      image_side: right
      greeting: "Call me Os"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: false
      cta_buttons:
        - text: View My Work
          url: "#all-publications"
          icon: arrow-down
        - text: Download CV
          url: "/uploads/Os_CV.pdf"
          new_tab: true
          icon: arrow-down-tray
        - text: Get In Touch
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["0rem", "0", "4rem", "0"]
  
  # Filterable Portfolio - Alpine.js powered project filtering
    # - block: portfolio
    #   id: projects
    #   content:
    #     title: "Featured Publications"
    #     subtitle: "A selection of my recent work"
    #     count: 0
    #     featured_only: true
    #     filters:
    #       folders:
    #         - projects
    #     buttons:
    #       - name: All
    #         tag: '*'
    #       - name: Multimodal Learning
    #         tag: Multimodal Learning
    #       - name: Egocentric Vision
    #         tag: Egocentric Vision
    #       - name: Action Recognition
    #         tag: Action Recognition
    #       - name: World Modelling
    #         tag: World Modelling
    #       - name: Self-supervised Learning
    #         tag: Self-supervised Learning
    #       - name: LLMs
    #         tag: LLMs
    #     default_button_index: 0
    #     # Archive link auto-shown if more projects exist than 'count' above
    #     # archive:
    #     #   enable: false  # Set to false to explicitly hide
    #     #   text: "Browse All"  # Customize text
    #     #   link: "/work/"  # Custom URL
    #   design:
    #     columns: 3
    #     background:
    #       color:
    #         light: "#ffffff"
    #         dark: "#0d0d12"
    #     spacing:
    #       padding: ["4rem", "0", "4rem", "0"]

  # All Publications - Vertical publication list with media and links
  - block: all-publications
    id: all-publications
    content:
      title: "📚 Publications"
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Multimodal Learning
          tag: Multimodal Learning
        - name: Egocentric Vision
          tag: Egocentric Vision
        - name: Action Recognition
          tag: Action Recognition
        - name: World Modelling
          tag: World Modelling
        - name: Self-supervised Learning
          tag: Self-supervised Learning
        - name: LLMs
          tag: LLMs
        - name: Datasets
          tag: Datasets
        - name: Semantic Segmentation
          tag: Semantic Segmentation
        - name: Pose Estimation
          tag: Pose Estimation
      default_button_index: 0
      count: 0
      sort_by: Date
      sort_ascending: false
    design:
      background:
        color:
          light: "#ffffff"
          dark: "#111827"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # # Visual Tech Stack - Icons organized by category
  # - block: tech-stack
  #   id: skills
  #   content:
  #     title: "Tech Stack"
  #     subtitle: "Technologies I use to build things"
  #     categories:
  #       - name: Languages
  #         items:
  #           - name: TypeScript
  #             icon: devicon/typescript
  #           - name: JavaScript
  #             icon: devicon/javascript
  #           - name: Python
  #             icon: devicon/python
  #           - name: Go
  #             icon: devicon/go
  #       - name: Frontend
  #         items:
  #           - name: React
  #             icon: devicon/react
  #           - name: Next.js
  #             icon: devicon/nextjs
  #           - name: Tailwind CSS
  #             icon: devicon/tailwindcss
  #           - name: Alpine.js
  #             icon: devicon/alpinejs
  #       - name: Backend
  #         items:
  #           - name: Node.js
  #             icon: devicon/nodejs
  #           - name: Express
  #             icon: devicon/express
  #           - name: PostgreSQL
  #             icon: devicon/postgresql
  #           - name: Redis
  #             icon: devicon/redis
  #       - name: DevOps
  #         items:
  #           - name: Docker
  #             icon: devicon/docker
  #           - name: AWS
  #             icon: devicon/amazonwebservices-wordmark
  #           - name: GitHub Actions
  #             icon: brands/github
  #           - name: Vercel
  #             icon: devicon/vercel
  #   design:
  #     style: grid
  #     show_levels: false
  #     background:
  #       color:
  #         light: "#f5f5f5"
  #         dark: "#08080c"
  #     spacing:
  #       padding: ["4rem", "0", "4rem", "0"]
  
  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: "💼 Experience"
      date_format: Jan 2006
      items:
        - title: AI Research Scientist Intern
          company: Meta Reality Labs
          company_url: ''
          company_logo: ''
          location: Zurich, Switzerland
          date_start: '2025-05-01'
          date_end: '2025-11-30'
          description: |2-
            * Created a novel dataset and benchmark, and developed a multimodal large language model for robust perception of human states.
            * Published research paper as first-author in CVPR 2026.
        - title: Computer Vision Research Scientist
          company: SpreeAI
          company_url: ''
          company_logo: ''
          location: Nevada, USA
          date_start: '2022-07-01'
          date_end: '2023-02-28'
          description: |2-
            * Developed a conditional diffusion model that enhanced high-quality user face reconstruction, resulting in a 20% improvement in performance compared to previous methods.
            * Innovated a U-Net architecture for head swapping that preserved pose, skin tone, and illumination, improving realism in AI-powered photorealistic try-on.
        - title: Deep Learning Intern (Prof. Mohamed Elhoseiny, Vision-CAIR Group)
          company: King Abdullah University of Science and Technology (KAUST)
          company_url: ''
          company_logo: ''
          location: Thuwal, Saudi Arabia
          date_start: '2022-03-01'
          date_end: '2023-01-31'
          description: |2-
            * Led the collection of the first and largest vision-language dataset with affective captions and explanations in four languages.
            * Co-developed training techniques and recipes for leveraging diversity of language and culture towards superior performance in image captioning and emotion prediction tasks.
            * Co-authored and published a high-impact paper at EMNLP 2022.
        - title: Remote Visiting Research Student (Prof. Sarah Bargal, IVC Group)
          company: Boston University
          company_url: ''
          company_logo: ''
          location: Boston, USA
          date_start: '2021-06-01'
          date_end: '2021-12-31'
          description: |2-
            * Designed and implemented data augmentation pipelines tailored to preserve object characteristics and dataset diversity.
            * Delivered insights into the challenges of balancing datasets and optimizing segmentation performance in deformable industrial waste objects.
            * Co-authored and published a pioneering paper at CVPR 2022.
    design:
      columns: '1'
      background:
        color:
          light: "#f5f5f5"
          dark: "#0b1220"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Education Timeline
  - block: resume-education
    id: education
    content:
      title: "🎓 Education"
      date_format: Jan 2006
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#111827"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Awards Timeline
  - block: resume-awards
    id: awards
    content:
      title: "🏆 Awards"
    design:
      columns: '1'
      background:
        color:
          light: "#f5f5f5"
          dark: "#0b1220"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Teaching Timeline
  - block: resume-teaching
    id: teaching
    content:
      title: "📖 Teaching"
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#111827"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: "✉️ Get In Touch"
      text: |-
        I am always happy to discuss research collaborations, internships, and full-time opportunities in computer vision and multimodal learning.
        If you are hiring, collaborating, or want to chat about ideas, feel free to reach out.
      email: mohamed.abdelfattah@epfl.ch
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#f5f5f5"
          dark: "#0b1220"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # CTA Card
  - block: cta-card
    content:
      title: "🚀 Open to Opportunities"
      text: |-
        I'm currently looking for **research** roles in industry or academia.
        
        Let's connect and discuss how I can help your team.
      button:
        text: 'Download Resume'
        url: "https://moo-osama.github.io/imgs_main/Os_CV.pdf"
        new_tab: true
    design:
      card:
        # Light mode: soft pastel theme gradient | Dark mode: rich deep gradient
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#ffffff"
          dark: "#111827"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
