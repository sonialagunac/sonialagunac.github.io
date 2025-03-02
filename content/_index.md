---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: rose-petals-blue.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  # - block: resume-awards
  #   id: news
  #   content:
  #     title: '🗞️ Recent News'
  #     text: '<a href="/news" style="text-decoration: underline;">See all News >></a>'
  #     # description: '[All news >>](/news)'
  #     # Note: `username` refers to the user's folder name in `content/authors/`
  #     username: admin
  - block: collection
    id: news
    content:
      title: '🗞️ Recent News'
      text: '<a href="news" style="text-decoration: underline;">See all News >></a>'
      subtitle: ''
      # Page type to display. E.g. post, talk, publication...
      # page_type: news_col
      # Choose how many pages you would like to display (0 = all pages)
      count: 6
      # Filter on criteria
      filters:
        # author: ""
        # category: ""
        # tag: ""
        # exclude_featured: false
        # exclude_future: false
        # exclude_past: false
        # publication_type: ""
        folders:
          - news
        # featured_only: true
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: article-grid #play with data-title-summary #citation # change to data-title-summary, also cute
      # Reduce spacing
      # spacing:
      #   padding: [0, 0, 0, 0]

    # design:
    #   spacing:
    #     padding: [0, 0, 0, 0]   # Removes internal padding
    #     margin: [0, 0, 0, 0]    # Removes external margin
  # - block: cta-card
  #   id: more-news
  #   content:
  #     title: 
  #     text:
  #     button:
  #       text: "See More News >>"
  #       url: news  # This should match the slug of your full news page
  #   design:
  #     card:
  #       css_class: "bg-dark"
  #       # css_style: "height: 20px; min-height: 20px; line-height: 20px;"
  #     button:
  #       style: "background-color: #444; color: white; border-radius: 6px; padding: 5px 10px;"
  #       hover_style: "background-color: #555; color: white;"
  #     spacing:
  #       padding: [0, 0, 0, 0]  
  #       margin: [0, 0, 0, 0]   # Removes all extra margin
        # Removes unnecessary spacing
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  - block: collection
    id: publications
    content:
      title: 📝 Featured Publications
      # text: '<a href="/publications" style="text-decoration: underline;">See All Publications >> or checkout my Scholar Profile</a>'
      # text: 'See <a href="publications" style="text-decoration: underline;"> All Publications >></a> or checkout my Google Scholar Profile'
      text: '<a href="publication" style="text-decoration: underline;">See all Publications >></a> or checkout my <a href="https://scholar.google.com/citations?user=PljVnCQAAAAJ&hl=es&oi=ao" style="text-decoration: underline;">Google Scholar >></a>'
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: citation #article-grid
      # columns: 2
      # spacing:
      #   padding: [0, 0, 0, 0]  # Remove internal padding inside the block
      #   margin: [0, 0, 0, 0]  # Reduce top margin to 20px, remove other
  # - block: collection
  #   # id: publicationslong
  #   content:
  #     title: Publications
  #     count: 0
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation

  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  # - block: collection
  #   id: news
  #   content:
  #     title: Professional Experience
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
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
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]

  #  - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---