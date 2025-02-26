---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    id: positions
    content:
      title: Positions
      # Date format for experience
      # Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Add/remove as many `experience` items below as you like.
      # Required fields are `title`, `company`, and `date_start`.
      # Leave `date_end` empty if it's your current employer.
      # Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      # Here the number indcates the indentation
      items:
        - title: Postdoctoral Researcher
          company: University of Pennsylvania
          # company_url: 
          company_logo: upenn-logo
          location: Philadelphia (USA)
          date_start: '2022-03-01'
          date_end: ''
          description: |2-
            - 2023-02 -- present: Postdoc in the group of Professor [Gene Mele](https://live-sas-physics.pantheon.sas.upenn.edu/people/standing-faculty/eugene-mele).
            - 2022-03 -- 2023-02: Visiting Scholar in the Group of Professor [Gene Mele](https://live-sas-physics.pantheon.sas.upenn.edu/people/standing-faculty/eugene-mele) supported by an [INTER Mobility grant](https://www.fnr.lu/results-2021-2-inter-mobility-call/) of the Luxembourg National Research Fund (FNR).
        - title: Postdoctoral Researcher
          company: University of Luxembourg
          # company_url: 
          company_logo: unilu-logo
          location: Luxembourg (Luxembourg)
          date_start: '2020-10-01'
          date_end: '2022-02-28'
          description: |2-
            - Postdoc in the group of Professor [Thomas Schmidt](https://www.tmqs.lu).  
          # - Main research topic: Artifical event horizons in Weyl semimetals.
        - title: Postdoctoral Researcher
          company: Technical University of Braunschweig
          # company_url: 
          company_logo: tubs-logo
          location: Braunschweig (Germany)
          date_start: '2018-04-01'
          date_end: '2020-09-30'
          description: |2-
            - Postdoc in the group of Professor [Patrik Recher](https://www.tu-braunschweig.de/en/imaph/rechergroup).
          # - Main research topic: Topological scattering networks and mesoscopic transport in twisted bilayer graphene.
    design:
      columns: '2'
  - block: collection
    id: publications
    content:
      title: Publications
      # text: |-
      #   {{% callout note %}}
      #   Quickly discover relevant content by [filtering publications](./publication/).
      #   {{% /callout %}}
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
        # - name: All
        #   tag: '*'
        - name: Research
          tag: research
        - name: Errata
          tag: errata
        - name: GitHub
          tag: github
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Choose a layout view
      view: compact
      # view: showcase
      # # For Showcase view, flip alternate rows?
      # flip_alt_rows: false
  # - block: collection
  #   id: posts
  #   content:
  #     title: Posts
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
  # - block: collection
  #   id: talks
  #   content:
  #     title: Talks #Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  - block: contact
    id: contact
    content:
      title: Contact
      # subtitle:
      # text: |-
      #   Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: cdebeule@upenn.edu #[cdebeule@upenn.edu](mailto:cdebeule@upenn.edu)
      # phone: ''
      # appointment_url: ''
      contact_links:
        # - icon: researchgate
        #   icon_pack: ai
        #   name: ResearchGate
        #   link: https://www.researchgate.net/profile/Christophe-De-Beule-2
        - icon: map-marker
          icon_pack: fas
          name: Department of Physics and Astronomy, University of Pennsylvania, Philadelphia, Pennsylvania 19104, USA
          link: https://www.physics.upenn.edu/
      #   - icon: twitter
      #     icon_pack: fab
      #     name: DM Me
      #     link: 'https://twitter.com/Twitter'
      #   - icon: skype
      #     icon_pack: fab
      #     name: Skype Me
      #     link: 'skype:echo123?call'
      #   - icon: video
      #     icon_pack: fas
      #     name: Zoom Me
      #     link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # address: 
      #   # building: David Rittenhouse Laboratory
      #   # institution: University of Pennsylvania
      #   street: 'Department of Physics & Astronomy, University of Pennsylvania, 209 South 33rd Street'
      #   city: Philadelphia
      #   region: Pennsylvania
      #   postcode: PA 19104
      #   country: United States
        # country_code: US
      # directions: ''
      # office_hours:
        # - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      # coordinates:
      #   latitude: '39.9519406'
      #   longitude: '-75.1899723'  
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: true
    design:
      columns: '2'
  # - block: skills
  #   content:
  #     title: Skills
  #     text: ''
  #     # Choose a user to display skills from (a folder name within `content/authors/`)
  #     username: admin
  #   design:
  #     columns: '1'
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://docs.hugoblox.com/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         icon: coursera
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         icon: edx
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         icon: datacamp
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'    
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
---
