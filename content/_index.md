---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: 李文鹏
      image:
        filename: hero-academic.png
      cta:
        label: '**查看项目**'
        url: '#projects'
      cta_alt:
        label: 联系我
        url: '#contact'
      text: |-
        **路径规划 · 运筹优化算法工程师**

        清华大学物流工程硕士 · 聚焦仓储机器人调度、智能堆场优化与物流运筹算法工程落地
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
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
        - title: 运筹优化算法工程师
          company: 招商局金融科技有限公司
          company_url: ''
          company_logo: org-gc
          location: 深圳南山
          date_start: '2025-07-01'
          date_end: '2026-01-31'
          description: |2-
              隶属于 AI 平台研发部，主导招商局集团交通物流业务的运筹优化算法体系建设：

              * 覆盖智能堆场、集装箱空箱调度、船舶订单管理及收箱找位等核心场景
              * 成功上线智能堆场位分配算法
              * 前瞻性布局运筹大模型（ORLM）在集团业务场景的落地
              * 针对集装箱预配载问题（CPMP）开展理论预研与技术验证

        - title: 运筹优化算法工程师
          company: 深圳市库宝软件有限公司（海柔机器人）
          company_url: 'https://www.hairobotics.com/'
          company_logo: org-gc
          location: 深圳宝安
          date_start: '2022-03-01'
          date_end: '2024-11-30'
          description: |2-
              隶属于海柔软件部算法组：

              * 主导多机器人调度系统路径规划模块的死锁解锁算法，提升搬箱效率与订单履约效率
              * 参与任务分配模块开发，优化多机型 A61 机器人库位选择及多背篓料箱机器人回库策略
              * 深度参与安全马甲定位算法开发，完成调度系统接入

        - title: 技术支持 · 算法专家（外派）
          company: HAI Robotics EMEA
          company_url: 'https://www.hairobotics.com/'
          company_logo: org-x
          location: 荷兰阿姆斯特丹
          date_start: '2023-07-01'
          date_end: '2024-01-31'
          description: |2-
              2023 年 7 月作为软件算法代表外派至欧洲分公司：

              * 完成输送线、安全马甲、安全门等调度系统设备的接入与调试
              * 与欧洲客户联调上下游设备对接，推动项目快速上线
              * 支持欧洲软件团队培训体系建设，搭建知识库，达成外派目标后归国
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
          description: 清华大学院研究生院二等奖学金
          icon: award
          organization: 清华大学
          organization_url: https://www.tsinghua.edu.cn/
          title: 研究生院二等奖学金
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2019-01-01'
          description: 清华大学研究生院优秀学生干部
          icon: users
          organization: 清华大学
          organization_url: https://www.tsinghua.edu.cn/
          title: 优秀学生干部
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2014-01-01'
          description: 国家励志奖学金、成绩优秀奖、一等奖学金（多次）
          icon: award
          organization: 北京信息科技大学
          organization_url: ''
          title: 国家励志奖学金
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2021-07-01'
          description: 基于元胞自动机的移动机器人履行系统仿真分析
          icon: graduation-cap
          organization: 清华大学
          organization_url: https://www.tsinghua.edu.cn/
          title: 硕士毕业论文
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
        - name: 运筹优化
          tag: Operations Research
        - name: 机器人调度
          tag: Robotics
        - name: 机器学习
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
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        欢迎就路径规划、运筹优化或算法工程相关机会与我联系。
      email: lwp01@qq.com
      phone: '+86 186 1703 3167'
      address:
        street: 工业六路12号鸣溪谷6A501
        city: 深圳市南山区
        region: 广东省
        postcode: ''
        country: 中国
        country_code: CN
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: 'https://www.linkedin.com/in/wenpeng-li-2aa689121/'
        - icon: github
          icon_pack: fab
          name: GitHub
          link: 'https://github.com/flying2322'
        - icon: graduation-cap
          icon_pack: fas
          name: Google Scholar
          link: 'https://scholar.google.co.uk/citations?user=krKEnn4AAAAJ&hl=nl'
      coordinates:
        latitude: '22.4833'
        longitude: '113.9167'
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
