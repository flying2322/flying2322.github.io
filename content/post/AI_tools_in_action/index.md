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

this is a test file to check whether post articale was display as wishes.

正文用 Markdown 写即可，支持代码高亮、公式、图表等。

```python
def plan_path(start, goal):
    return [start, goal]
```


## AI tools in action

最近工作的缘故尝试了多款AI工具，趁着这个周末记录一下使用的感受。
首先让我产生振动和吃惊的第一个工具是cursor，我主要使用的是ubuntu系统下的deb。最新的版本号是：3.10.20，升级于7月9日

其能力已经有些超出我的想象了，代码能力及其强大，可以：
1. 快速理解整个几万行代码的项目。
2. 生成主要函数和模块的调用图
3. 直接改bug和代码提交
4. 直接分支管理
使用下来的体感还是很明显的，提效很多，几乎可以快速进行理解用户需求并快速实现，甚至上线了多Agent模式，之前的中中的中毒终端在值中

