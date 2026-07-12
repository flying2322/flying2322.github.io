这是一个典型的 Hugo Academic 主题（或 Wowchemy）的网站。这个主题是**数据驱动**的，你主要通过编辑配置文件和特定的 Markdown 文件来控制首页内容，而不是去写复杂的 HTML 代码。
针对你提到的各个板块，对应的修改位置如下：
### 1. 基本信息、技能、经验、成就
这部分通常由一个特定的用户主页文件控制。根据你的目录结构，你需要关注 `content/authors/admin/` 这个文件夹（`admin` 是默认的用户 ID）：
*   **修改文件**：`content/authors/admin/_index.md`
*   **如何操作**：
    *   打开这个文件，你会在顶部看到类似 `title: "你的名字"` 和 `role: "你的职位"` 的信息。
    *   **Biography（简介）**: 直接编辑文件正文部分的文字内容。
    *   **Interests（兴趣/技能）**: 在 `interests` 字段后添加列表项。
    *   **Education（教育背景）**: 在 `education` 字段下添加课程和学校。
    *   **Experience（工作经验）**: 在 `experience` 字段下添加工作经历。
    *   **Accomplishments/Skills（成就/技能）**: 通常对应的字段是 `skills` 或 `awards`。
### 2. 精选项目
Projects 页面展示的是 `content/project/` 目录下的内容。
*   **控制位置**：`content/project/`
*   **如何操作**：
    *   每个子文件夹（如 `example` 和 `external-project`）就是一个项目。
    *   **修改内容**：编辑文件夹里的 `index.md`，修改标题、摘要、链接等。
    *   **增减项目**：在 `content/project/` 下新建文件夹并放入 `index.md` 即可新增；删除文件夹即可移除。
    *   **图片**：文件夹内的 `featured.jpg` 或 `featured.png` 就是封面图。
    *   **设置精选**：在 `index.md` 的顶部参数中，通常可以通过 `featured = true` 来控制它是否以大图形式显示在特定位置。
### 3. 最新文章
Posts 页面展示的是 `content/post/` 目录下的内容。
*   **控制位置**：`content/post/`
*   **如何操作**：
    *   和 Projects 类似，每个子文件夹（如 `blog-with-jupyter`）就是一篇文章。
    *   **发布/隐藏**：在文章的 `index.md` 顶部参数中，设置 `draft: true` 可以隐藏草稿，设为 `false` 或删除该行即可发布。首页会自动列出最新的文章。
### 4. 精选出版物
Publications 页面展示的是 `content/publication/` 目录下的内容。
*   **控制位置**：`content/publication/`
*   **如何操作**：
    *   子文件夹（如 `conference-paper`）代表一个出版物。
    *   **引用文件**：文件夹里的 `cite.bib` 是参考文献数据，用于生成标准的引用格式。
    *   **PDF文件**：`conference-paper.pdf` 会被自动关联，提供下载按钮。
    *   **详情**：编辑 `index.md` 来修改标题、作者和摘要。
### 5. 图库
Gallery 对应的是 `assets/media/albums/`。
*   **控制位置**：`assets/media/albums/`
*   **如何操作**：
    *   根据你的目录结构 `albums/demo // All the pictures in Gallery shows here`，你需要把想要展示的图片放到 `assets/media/albums/demo/` 目录下。
    *   Hugo 会自动扫描这个目录并在图库组件中生成缩略图。
### 6. 全局样式与菜单
如果你觉得以上改完后首页顺序还是不对，或者想关闭某个板块：
*   **修改文件**：`config/_default/params.yaml`
*   **关键参数**：在这个文件中，你通常能找到 `main_sections` 或 `homepage` 相关的配置，用来决定首页优先显示哪个文件夹的内容（是 `post` 还是 `publication`）。
**总结一下：**
*   **改个人信息**：去 `content/authors/admin/_index.md`
*   **改页面列表**：去对应的 `content/post/`、`content/project/` 等文件夹删减或编辑文件。
*   **改图片**：把图片放到对应的文件夹或替换原有的 `featured.jpg`。
修改完保存后，你在本地运行 Hugo 服务器应该就能实时看到变化了。

---
## 项目概览

这是基于 **Hugo + Hugo Blox（原 Wowchemy Academic）** 的个人学术/技术主页，部署在 **GitHub Pages**（`https://flying2322.github.io`）。

核心特点：

- **内容驱动**：主要改 Markdown + YAML 配置，不写复杂 HTML
- **单页首页**：`content/_index.md` 用多个 `block` 拼出 About、Experience、Posts、Projects 等区块
- **自动部署**：推送到 `main` 分支后，`.github/workflows/publish.yaml` 会用 Hugo 构建并发布

当前站点已有一部分你的个人信息（Dominic Li、运筹算法工程师、海柔机器人等），但首页 Hero 区仍是模板默认文案，部分全局配置（如 `baseURL`）也还没完全改成你的域名。

---

## 一、撰写一篇新的科技博文

### 需要修改/新增的位置

在 `content/post/` 下**新建一个文件夹**，例如：

```
content/post/my-ai-article/
├── index.md          # 博文正文（必填）
└── featured.jpg      # 封面图（可选）
```

### 博文模板示例

```markdown
---
title: 多智能体路径规划实践笔记
subtitle: 从理论到仓库机器人落地
summary: 记录 MAPF 算法在仓储场景中的工程化经验。
date: '2026-07-12T00:00:00Z'
lastmod: '2026-07-12T00:00:00Z'
draft: false          # true = 草稿，不发布
featured: false       # true = 首页「精选」展示

authors:
  - admin             # 对应 content/authors/admin/

tags:
  - Robotics
  - Algorithm

categories:
  - Tech

# 可选：关联到某个项目
projects:
  - example

image:
  caption: '封面说明'
  focal_point: Smart
  placement: 2

# 写技术文时可开启
math: false
---

正文用 Markdown 写即可，支持代码高亮、公式、图表等。

```python
def plan_path(start, goal):
    return [start, goal]
```

## 小节标题

更多内容...
```

### 参考现有示例

| 用途 | 文件 |
|------|------|
| 基础博文结构 | `content/post/getting-started/index.md` |
| 技术写作（代码、公式、图表） | `content/post/writing-technical-content/index.md` |
| Jupyter 博文 | `content/post/blog-with-jupyter/index.md` |

### 发布后如何显示

- 导航栏 **Posts** → 首页 `#posts` 区块（`content/_index.md` 里 `block: collection`，`folders: [post]`）
- 设置 `draft: false` 才会发布
- 设置 `featured: true` 可突出展示
- `date` 越新，排序越靠前

---

## 二、更新工作与项目经历

工作经历和项目分布在**两个层级**，建议都维护。

### 1. 个人档案（About 区块）

**文件：** `content/authors/admin/_index.md`

这里控制首页 **Biography / Skills** 以及博文作者信息：

| 字段 | 作用 |
|------|------|
| `title` / `role` | 姓名、职位 |
| `bio` | 简短简介 |
| 正文 Markdown | About 区长介绍 |
| `organizations` | 当前单位/链接 |
| `interests` | 研究方向/兴趣 |
| `education` | 教育背景 |
| `skills` | 技能条 |
| `social` | GitHub、LinkedIn、简历链接等 |

头像放在同目录：`content/authors/admin/avatar.jpg`。

### 2. 首页工作经历（Experience 区块）

**文件：** `content/_index.md`（约第 53–88 行）

在 `block: experience` → `items` 下增删条目：

```yaml
- title: Operations Research Algorithm Engineer
  company: Hai Robotics
  company_url: 'hairobotics.com'
  company_logo: org-gc      # 图标在 assets/media/icons/brands/
  location: Shenzhen
  date_start: '2022-03-22'
  date_end: ''              # 空 = 至今
  description: |2-
      * 路径规划算法
      * UWB 定位
```

新增一段工作，就复制一个 `- title: ...` 块；`date_end` 留空表示在职。

### 3. 项目经历（Projects 区块）

**目录：** `content/project/`

每个子文件夹 = 一个项目，例如 `content/project/warehouse-robot/`：

```markdown
---
title: 仓储机器人路径规划系统
summary: 面向多 AGV 的实时避障与调度。
tags:
  - Robotics
  - Demo          # 对应首页筛选标签
date: '2024-06-01T00:00:00Z'
external_link: ''  # 填 URL 则跳转到外部，不显示详情页

links:
  - icon: github
    icon_pack: fab
    name: Code
    url: https://github.com/xxx

image:
  caption: 项目截图
  focal_point: Smart
---

项目详细描述（Markdown）...
```

操作方式：

- **新增项目**：新建文件夹 + `index.md` + 可选 `featured.jpg`
- **修改项目**：编辑对应 `index.md`
- **删除项目**：删除整个文件夹
- **首页筛选**：`tags` 需与 `content/_index.md` 里 `block: portfolio` 的 `buttons` 一致（如 `Deep Learning`、`Demo`）

参考：`content/project/example/index.md`、`content/project/external-project/index.md`。

### 4. 成就/证书（可选）

**文件：** `content/_index.md` 中 `block: accomplishments`（约第 89–130 行）

证书、课程、奖项等在这里维护。

---

## 三、其他你可能要改的文件

| 文件 | 用途 |
|------|------|
| `config/_default/hugo.yaml` | 站点名（当前 `PandaBoy`）、`baseURL`（建议改为 `https://flying2322.github.io/`） |
| `config/_default/menus.yaml` | 顶部导航顺序与链接 |
| `config/_default/params.yaml` | 主题、字体、SEO、评论等全局设置 |
| `content/_index.md` | 首页各区块顺序、联系信息、Gallery 等 |
| `static/uploads/resume.pdf` | 菜单栏 CV 下载 |
| `assets/media/albums/demo/` | 图库照片 |

---

## 四、推荐工作流

1. **本地预览**（需安装 Hugo Extended）：
   ```bash
   cd /home/wp/flying2322.github.io
   hugo server
   ```
   浏览器打开 `http://localhost:1313` 实时查看。

2. **编辑内容**：
   - 新博文 → `content/post/新文件夹/index.md`
   - 工作/技能 → `content/authors/admin/_index.md` + `content/_index.md` 的 experience
   - 项目 → `content/project/新文件夹/index.md`

3. **发布**：提交并 push 到 `main`，GitHub Actions 自动构建部署。

---

## 五、快速对照表

| 你的需求 | 主要修改文件 |
|----------|--------------|
| 写一篇科技博文 | `content/post/<slug>/index.md` |
| 更新简介、技能、教育 | `content/authors/admin/_index.md` |
| 更新工作经历时间线 | `content/_index.md` → `experience` 区块 |
| 更新/新增项目 | `content/project/<项目名>/index.md` |
| 更新证书/成就 | `content/_index.md` → `accomplishments` 区块 |
| 更新联系方式 | `content/_index.md` → `contact` 区块 |
| 更新简历 PDF | `static/uploads/resume.pdf` |
| 改站点名/域名 | `config/_default/hugo.yaml` |

如果你愿意，我可以直接帮你：新建一篇博文模板、更新某段工作经历，或把 `baseURL`/首页 Hero 改成你的个人介绍。说一下具体内容即可。