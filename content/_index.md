---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
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
  - block: collection
    id: featured
    content:
      title: Job market paper
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent working papers
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
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
        - name: England
          tag: England
        - name: Germany
          tag: Germany
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  # - block: features
  #   content:
  #     title: Curriculum Vitae 
  #     items:   
  #       - name: ''
  #         description: 
  #         icon: page
  #         icon_pack: python 
  #       - name: Pdf version {{% staticref "uploads/resume.pdf" %}}Download here {{% /staticref %}}
  #         description: 
  #         icon: page
  #         icon_pack: python                 
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  - block: experience
    content:
      title: Short CV
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Assistant Professor
          company: University of Southern Denmark
          description: At the Department of Economics and part of the Historical Economics and Development Group (HEDG group) 
          company_logo: uni
          location: Odense, Denmark
          date_start: '2024-08-15'
        - title: PhD in Economic History
          company: London School of Economics
          company_url: ''
          company_logo: uni
          location: London, UK
          date_start: '2019-09-01'
          date_end: '2024-04-30'
          description: 'Thesis title: On the Shoulders of Science - Early Science as a Driver of Innovation During the Early Industrial Revolution
          

          Supervisors: Prof. Max-Stephan Schulze and Dr. Jeremiah Dittmar'
        - title: Visiting scholar
          company: Northwestern University
          company_url: ''
          company_logo: uni
          location: Evanston, IL, USA
          date_start: '2022-09-01'
          date_end: '2022-12-31'
          description: Visiting scholar at the Department of Economics, hosted by Prof. Joel Mokyr
        - title: MSc Economic History (Research)
          company: London School of Economics
          company_url: ''
          company_logo: uni
          location: London, UK
          date_start: '2018-09-01'
          date_end: '2019-09-01'
          description: 
        - title: BA Philosophy & Economics
          company: University Bayreuth
          company_url: ''
          company_logo: uni
          location: Bayreuth, Germany
          date_start: '2013-10-01'
          date_end: '2017-09-01'
          description: 
    design:
      columns: '2'
  - block: features
    id: cvlong
    content:
      title: Curriculum Vitae 
      items:   
        - name: ''
          description: 
          icon: page
          icon_pack: python 
        - name: Pdf version {{% staticref "uploads/resume.pdf" %}}Download here {{% /staticref %}}
          description: 
          icon: page
          icon_pack: python     
  - block: features
    content:
      title: Skills
      items:
        - name: Python
          description: Data analysis, natural language processing
          icon: python
          icon_pack: fab
        - name: R
          description: Data analysis, simulations, regression analysis
          icon: r-project
          icon_pack: fab
        - name: Stata
          description: Regression analysis
          icon: chart-line
          icon_pack: fas
        - name: ArcGIS
          description: Spatial analysis
          icon: globe
          icon_pack: fas   
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
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        
      # Contact (add or remove contact options as necessary)
      email: j.koschnick@lse.ac.uk
      #phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      office_hours:
        - 'no available office hours at the moment'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/juliuskoschnick'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
