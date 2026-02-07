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