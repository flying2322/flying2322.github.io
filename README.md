

## Note

### 2026.2.7
- [Done] 2026.2.7 修复了域名过长，和github仓库名不一致的问题
- Modify details important
  
### 2024.4.19
- 第一次部署成功，但是域名有点奇怪：https://flying2322.github.io/dominicli.github.io/ 希望简短好记一些。或许想办法申请下来：dominic.cn
- 大致浏览了Hugo个人网页部署 文件的目录结构
- 删除之前通过netlify部署的内容，保留本网站并长期维护，书写博客之地。

### 20 April, 2024
. Folder hierearchy
```bash
├── LICENSE.md
├── README.md
├── academic.Rproj
├── assets
│   └── media 
│       ├── albums
│       │   └── demo    // All the pictures in Gallery shows here
│       ├── hero-academic.png 
│       ├── icon.png
│       └── icons
│           └── brands
├── config
│   └── _default
│       ├── hugo.yaml
│       ├── languages.yaml
│       ├── menus.yaml
│       ├── module.yaml
│       └── params.yaml
├── content
│   ├── _index.md
│   ├── authors
│   │   ├── _index.md
│   │   └── admin
│   │       ├── _index.md
│   │       ├── avatar.jpg
│   │       ├── avatar1.jpg
│   │       ├── avatar2.jpg
│   │       └── event
│   ├── post
│   │   ├── _index.md
│   │   ├── blog-with-jupyter
│   │   │   ├── featured.png
│   │   │   ├── index.md
│   │   │   └── output_1_0.png
│   │   ├── getting-started
│   │   │   ├── featured.jpg
│   │   │   └── index.md
│   │   └── writing-technical-content
│   │       ├── featured.jpg
│   │       ├── index.md
│   │       ├── line-chart.json
│   │       └── results.csv
│   ├── privacy.md
│   ├── project
│   │   ├── example
│   │   │   ├── featured.gif
│   │   │   └── index.md
│   │   └── external-project
│   │       ├── featured.jpg
│   │       └── index.md
│   ├── publication
│   │   ├── _index.md
│   │   ├── conference-paper
│   │   │   ├── cite.bib
│   │   │   ├── conference-paper.pdf
│   │   │   ├── featured.jpg
│   │   │   └── index.md
│   │   ├── journal-article
│   │   │   ├── cite.bib
│   │   │   ├── featured.jpg
│   │   │   └── index.md
│   │   └── preprint
│   │       ├── featured.jpg
│   │       └── index.md
│   ├── slides
│   │   └── example
│   │       └── index.md
│   └── terms.md
├── data
│   ├── fonts
│   ├── page_sharer.toml
│   └── themes
├── go.mod
├── images
│   ├── screenshot.png
│   └── tn.png
├── netlify.toml
├── preview.png
├── static
│   └── uploads
│       ├── resume.pdf
│       └── resumeDemo.pdf
└── theme.toml

32 directories, 52 files
```
