---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: "About Me"
      subtitle: ""
      text: |-
        I am a Doctor of Business Administration (DBA) researcher at the University of Wales Trinity Saint David, with research interests in digital transformation, artificial intelligence, social media and digital ethics, consumer behaviour, branding, and marketing strategy.

        My research explores how individuals and organisations navigate the opportunities and challenges created by emerging digital technologies. My current DBA research focuses on how social media users reconcile awareness of digital risks with continued platform use, examining issues related to privacy, trust, digital wellbeing, and online behaviour.

        Alongside my academic journey, I have professional experience in business development, brand communication, and marketing within the corporate sector.
    design:
      columns: "1"

  - block: markdown
    content:
      title: "Professional Summary"
      subtitle: ""
      text: |-
        Business professional and Doctor of Business Administration (DBA) researcher with experience in business development, brand communication, and marketing strategy.

        My professional background includes business growth initiatives, market analysis, stakeholder relationship management, and strategic planning within the corporate sector.

        I combine industry experience with academic research to explore digital transformation, artificial intelligence, organisational decision-making, consumer behaviour, and responsible technology adoption.
    design:
      columns: "1"
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
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
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
 
---