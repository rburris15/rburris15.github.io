---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      #button:
        #text: Download CV
        #url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 Career Goals'
      subtitle: ''
      text: |-
        I'm passionate about using data science and AI to create tools that simplify complex workflows and empower informed decision-making. I love turning data into actionable insights that help teams work more efficiently and strategically. Ultimately, I strive to make advanced analytics accessible and impactful across both technical and business domains.

        Please reach out to collaborate!
      button:
        text: Contact Me!
        url: mailto:rachaelburris15@gmail.com
    design:
      columns: '1'
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
      columns: 3
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
#  - block: collection
#    id: talks
#    content:
#      title: Recent & Upcoming Talks
#      filters:
#        folders:
#          - events
#    design:
#      view: card
#  - block: collection
#    id: news
#    content:
#      title: Recent News
#      subtitle: ''
#      text: ''
#      # Page type to display. E.g. post, talk, publication...
#      page_type: blog
#      # Choose how many pages you would like to display (0 = all pages)
#      count: 5
#      # Filter on criteria
#      filters:
#        author: ''
#        category: ''
#        tag: ''
#        exclude_featured: false
#        exclude_future: false
#        exclude_past: false
#        publication_type: ''
#      # Choose how many pages you would like to offset by
#      offset: 0
#      # Page order: descending (desc) or ascending (asc) date.
#      order: desc
 #   design:
 #     # Choose a layout view
 #     view: card
 #     # Reduce spacing
 #     spacing:
  #      padding: [0, 0, 0, 0]
---

