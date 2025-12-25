---
# Leave the homepage title empty to use the site title
title: ""
date: "2022-10-24"
type: landing


design:
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      background:
      css_class: bg-bio-light dark:bg-bio-dark



  - block: collection
    id: papers
    content:
      title: Latest Working Papers
      filters:
        folders:
          - publication
        publication_type: "3"
        featured_only: false
    design:
      view: card
      columns: 2

  - block: collection
    id: featured
    content:
      title: Publications and Working Papers
      text: |-
        
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
      columns: 2


  - block: markdown
    id: news
    content:
      title: News
      # Use the standard Hugo shortcode syntax
      text: "{{< tweet user=\"juliuskoschnick\" id=\"1942221220818399277\" >}}"


  - block: collection
    id: projects
    content:
      title: Threads
      filters:
        folders:
          - project
      buttons:
        - name: All
          tag: '*'
        - name: England
          tag: England
        - name: Germany
          tag: Germany
    design:
      view: article-grid
      columns: 2
      flip_alt_rows: false

  - block: experience
    content:
      title: Short CV
      date_format: Jan 2006
      items:
        - title: Assistant Professor
          company: University of Southern Denmark
          company_logo: uni
          location: Odense, Denmark
          date_start: '2024-08-15'
          description: At the Department of Economics, part of the Danish Institute of Advanced Study (DIAS) and of the Historical Economics and Development Group (HEDG)

        - title: PhD in Economic History
          company: London School of Economics
          company_logo: uni
          location: London, UK
          date_start: '2019-09-01'
          date_end: '2024-04-30'
          description: |-
            Thesis title: On the Shoulders of Science - Early Science as a Driver of Innovation During the Early Industrial Revolution

        - title: Visiting Scholar
          company: Northwestern University
          company_logo: uni
          location: Evanston, IL, USA
          date_start: '2022-09-01'
          date_end: '2022-12-31'
          description: Visiting scholar at the Department of Economics, hosted by Prof. Joel Mokyr

        - title: MSc Economic History (Research)
          company: London School of Economics
          company_logo: uni
          location: London, UK
          date_start: '2018-09-01'
          date_end: '2019-09-01'

        - title: BA Philosophy & Economics
          company: University Bayreuth
          company_logo: uni
          location: Bayreuth, Germany
          date_start: '2013-10-01'
          date_end: '2017-09-01'

    design:
      columns: 2


  - block: features
    content:
      title: Skills
      items:
        - name: NLP 
          description: Working with transformer models, model training, fine-tuning of large models, building economic indicators based on text data
        - name: Python
          description: Data analysis, natural language processing
        - name: R
          description: Data analysis, simulations, regression analysis
        - name: Stata
          description: Regression analysis
        - name: ArcGIS
          description: Spatial analysis




  - block: markdown
    content:
      title: Contact
      text: |-
        Email: [juko@sam.sdu.dk](mailto:juko@sam.sdu.dk)

        [Twitter DM](https://twitter.com/juliuskoschnick)

        No office hours at the moment.
    design:
      columns: 2
---
