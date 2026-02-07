# [Hugo Academic CV Theme](https://github.com/HugoBlox/theme-academic-cv)

[![Screenshot](./preview.png)](https://hugoblox.com/templates/)

The Hugo **Academic Resumé Template** empowers you to easily create your job-winning online resumé, showcase your academic publications, and create online courses or knowledge bases to grow your audience.

[![Get Started](https://img.shields.io/badge/-Get%20started-ff4655?style=for-the-badge)](https://hugoblox.com/templates/)
[![Discord](https://img.shields.io/discord/722225264733716590?style=for-the-badge)](https://discord.com/channels/722225264733716590/742892432458252370/742895548159492138)  
[![Twitter Follow](https://img.shields.io/twitter/follow/GetResearchDev?label=Follow%20on%20Twitter)](https://twitter.com/GetResearchDev)

️**Trusted by 250,000+ researchers, educators, and students.** Highly customizable via the integrated **no-code, Hugo Blox Builder**, making every site truly personalized ⭐⭐⭐⭐⭐

Easily write technical content with plain text Markdown, LaTeX math, diagrams, RMarkdown, or Jupyter, and import publications from BibTeX.

[Check out the latest demo](https://academic-demo.netlify.app/) of what you'll get in less than 10 minutes, or [get inspired by our academics and research groups](https://hugoblox.com/creators/).

The integrated [**Hugo Blox Builder**](https://hugoblox.com) and CMS makes it easy to create a beautiful website for free. Edit your site in the CMS (or your favorite editor), generate it with [Hugo](https://github.com/gohugoio/hugo), and deploy with GitHub or Netlify. Customize anything on your site with widgets, light/dark themes, and language packs.

- 👉 [**Get Started**](https://hugoblox.com/templates/)
- 📚 [View the **documentation**](https://docs.hugoblox.com/)
- 💬 [Chat with the **Hugo Blox Builder community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@GetResearchDev](https://twitter.com/GetResearchDev) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithHugoBlox](https://twitter.com/search?q=%23MadeWithHugoBlox&src=typed_query)
- ⬇️ **Automatically import your publications from BibTeX** with the [Hugo Academic CLI](https://github.com/GetRD/academic-file-converter)
- 💡 [Suggest an improvement](https://github.com/HugoBlox/hugo-blox-builder/issues)
- ⬆️ **Updating?** View the [Update Guide](https://docs.hugoblox.com/reference/update/) and [Release Notes](https://github.com/HugoBlox/hugo-blox-builder/releases)

## We ask you, humbly, to support this open source movement

Today we ask you to defend the open source independence of the Hugo Blox Builder and themes 🐧

We're an open source movement that depends on your support to stay online and thriving, but 99.9% of our creators don't give; they simply look the other way.

### [❤️ Click here to become a GitHub Sponsor, unlocking awesome perks such as _exclusive academic templates and widgets_](https://github.com/sponsors/gcushen)

<p align="center"><a href="https://hugoblox.com/templates/" target="_blank" rel="noopener"><img src="https://hugoblox.com/uploads/readmes/academic_logo_200px.png" alt="Hugo Academic Theme for Hugo Blox Builder"></a></p>

## Demo image credits

- [Unsplash](https://unsplash.com)

## Latest news

<!--START_SECTION:news-->

- [Easily make an academic CV website to get more cites and grow your audience 🚀](https://hugoblox.com/blog/easily-make-academic-website/)
- [What&#39;s new in v5.2?](https://hugoblox.com/blog/whats-new-in-v5.2/)
- [What&#39;s new in v5.1?](https://hugoblox.com/blog/whats-new-in-v5.1/)
- [Version 5.0 (February 2021)](https://hugoblox.com/blog/version-5.0-february-2021/)
- [Version 5.0 Beta 3 (February 2021)](https://hugoblox.com/blog/version-5.0-beta-3-february-2021/)
<!--END_SECTION:news-->


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
