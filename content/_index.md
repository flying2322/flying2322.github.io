---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Operations Research Algorithm Engineer
          company: China Merchants Group Financial Technology
          company_url: ''
          company_logo: china-merchants
          location: Nanshan, Shenzhen
          date_start: '2025-07-01'
          date_end: '2026-01-31'
          description: |2-
              AI Platform R&D Department — led the OR optimization algorithm framework for CMG's transportation and logistics business:

              * Covered smart yard, empty container dispatch, vessel order management, and inbound slot recommendation
              * Successfully deployed smart yard slot allocation algorithm to production
              * Pioneered OR Large Language Model (ORLM) adoption across group business scenarios
              * Conducted theoretical research and technical validation on the Container Pre-Marshalling Problem (CPMP)

        - title: Operations Research Algorithm Engineer
          company: Shenzhen Kubao Software (HAI Robotics)
          company_url: 'https://www.hairobotics.com/'
          company_logo: hai-robotics
          location: Bao'an, Shenzhen
          date_start: '2022-03-01'
          date_end: '2024-11-30'
          description: |2-
              HAI Robotics Software Algorithm Team:

              * Led deadlock resolution algorithm for multi-robot path planning, improving tote-moving and order fulfillment efficiency
              * Contributed to task assignment module — optimized multi-model A61 robot slot selection and multi-tote robot return strategies
              * Deep involvement in safety vest positioning algorithm and scheduling system integration

        - title: Technical Support · Algorithm Specialist (Overseas)
          company: HAI Robotics EMEA
          company_url: 'https://www.hairobotics.com/'
          company_logo: hai-robotics
          location: Amsterdam, Netherlands
          date_start: '2023-07-01'
          date_end: '2024-01-31'
          description: |2-
              Dispatched as software algorithm representative to the European branch in July 2023:

              * Integrated and commissioned conveyor lines, safety vests, safety gates, and other scheduling system devices
              * Coordinated upstream/downstream equipment integration with European customers for rapid project go-live
              * Supported European software team training and knowledge base development; returned after achieving assignment goals
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2019-01-01'
          description: Graduate School Second-Class Scholarship
          icon: award
          organization: Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Graduate School Scholarship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2019-01-01'
          description: Outstanding Student Cadre, Tsinghua Graduate School
          icon: users
          organization: Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Outstanding Student Cadre
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2014-01-01'
          description: National Endeavor Scholarship, Academic Excellence Award, First-Class Scholarship (multiple)
          icon: award
          organization: Beijing Information Science & Technology University
          organization_url: ''
          title: National Endeavor Scholarship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2021-07-01'
          description: Simulation analysis of robotic mobile fulfillment system based on cellular automata
          icon: graduation-cap
          organization: Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Master's Thesis
          url: ''
    design:
      columns: '2'
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
        - name: Operations Research
          tag: Operations Research
        - name: Robotics
          tag: Robotics
        - name: Machine Learning
          tag: Machine Learning
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        Feel free to reach out regarding path planning, operations research, or algorithm engineering opportunities.

        <form action="https://formsubmit.co/lwp01@qq.com" method="POST" class="contact-form mt-4">
          <input type="hidden" name="_subject" value="New message from PandaBoy website">
          <input type="hidden" name="_captcha" value="false">
          <input type="hidden" name="_template" value="table">
          <input type="hidden" name="_next" value="https://flying2322.github.io/#contact">
          <div class="mb-3">
            <label class="form-label" for="contact-name">Name</label>
            <input class="form-control" type="text" id="contact-name" name="name" required>
          </div>
          <div class="mb-3">
            <label class="form-label" for="contact-email">Email</label>
            <input class="form-control" type="email" id="contact-email" name="email" required>
          </div>
          <div class="mb-3">
            <label class="form-label" for="contact-message">Message</label>
            <textarea class="form-control" id="contact-message" name="message" rows="5" required></textarea>
          </div>
          <button type="submit" class="btn btn-primary px-4">Send</button>
        </form>
    design:
      columns: '1'
---
