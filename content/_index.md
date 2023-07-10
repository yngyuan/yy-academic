---
# Leave the homepage title empty to use the site title
title: Yang(Zed) Yuan
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
      #   experience
        - title: Consultant
          company: Thoughtworks
          company_url: 'https://www.thoughtworks.com/'
          company_logo: org-x
          location: Shanghai, China
          date_start: '2021-08-16'
          date_end: ''
          description: Worked with some of the largest organisations in Asia-Pacific on their digital transformation journeys across domains including automotive, retail, and energy. Applied Design Thinking model and datat driven apporach to come with user centric product roadmaps. SAFe certified Scrum Master and Azure certified cloud practitioner.
    #   experience
        - title: Full-stack Developer, Practicum
          company: Dell Medical School
          company_url: 'https://dellmed.utexas.edu/'
          company_logo: org-x
          location: Austin, TX
          date_start: '2020-12-01'
          date_end: '2021-05-20'
          description: Design and developed a dashboard web app using Cube.js stack and the MIMIC-iii demo dataset. Co-created with doctors at the Dell Medical School, The application consists of a playground where doctors can try out different graphs with easy drag-and-drop operations, a demo data visualization of various graphs focusing on Sepsis, and a user account system providing customized dashboard for each account.

    #   experience
        - title: UX Researcher, Practicum
          company: Pop Social
          company_url: ''
          company_logo: org-x
          location: Austin, TX
          date_start: '2020-02-18'
          date_end: '2020-05-18'
          description: Led a team of 4 students to do User Experience research and Usability Testing. Initiated Heuristic Evaluation on POP Social App and made suggestions to enhance the User Experience. Owned competitive product analysis and presented with data visualization.

    #   experience
        - title: Data Analyst Intern 
          company: Tencent
          company_url: 'https://www.tencent.com/en-us/'
          company_logo: org-x
          location: Beijing, China
          date_start: '2018-05-21'
          date_end: '2028-09-30'
          description: Designed various A/B Tests and analyzed user behaviours and feed-backs for growth hacking of product. Built a Machine Learning model in Python, implementing Cluster Algorithms to draw App user profile. Owned and designed AARRR user acquisition analysis using HiveQL and Python.

        - title: Vendor Manager Intern
          company: Amazon
          company_url: 'https://www.amazon.com/'
          company_logo: org-x
          location: Beijing, China
          date_start: '2017-12-10'
          date_end: '2018-02-20'
          description: Implemented web crawlers to help make data-driven e-book onsite decisions and contributed to weekly campaigns of ”What’s worth reading” on Kindle book website.

    design:
      columns: '2'

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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: collection
    content:
      title: Recent Publications
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
#
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
#
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
#
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
#
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Well howdy there, partner! If you've got a question, a comment, or just wanna say Hi, don't be shy! Drop me a line and we'll see what trouble we can get into together. 
      # Contact (add or remove contact options as necessary)
      email: zedd.yuan@utexas.edu
      appointment_url: 'https://calendly.com'
      # address:
      #  street: 450 Serra Mall
      #  city: Stanford
      #  region: CA
      #  postcode: '94305'
      #  country: United States
      #  country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
