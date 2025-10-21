---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    content:
      title: Skills
      username: admin
    design:
      show_skill_percentage: false
  - block: resume-awards
    content:
      title: Awards
      username: admin
  - block: resume-languages
    content:
      title: Languages
      username: admin
  - block: markdown
    id: exp-header-img
    content:
      title: ""
      text: >-
        <figure style="max-width:60%; margin:0 auto;">
          <img
            src="/images/julius_koschnick.jpg"
            alt="Julius Koschnick at the Workshop on Technology and Long-Term Development at the University of Valencia"
            style="width:100%; height:auto; border-radius:0.5rem;"
            aria-describedby="exp-caption"
          />
          <figcaption
            id="exp-caption"
            style="text-align:center; font-size:0.875rem; color:#555;"
          >
            Presenting at the Workshop on Technology and Long-Term Development at the University of Valencia.
          </figcaption>
        </figure>
---
