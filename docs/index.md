# 欢迎来到集美大学机器人创新实验室博客首页

集美大学机器人创新实验室门户网站[jmurobot.com](https://www.jmurobot.com).

博客[github](https://github.com/YWwXxx/JMURobot-md)地址

[MkDocs](https://markdown-docs-zh.readthedocs.io/zh_CN/latest/)中文文档

该网站使用主题为[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)

网站托管于[ReadtheDocs](https://readthedocs.org/)

## 使用教程

在网页中发表博客

- git 项目到本地（推荐使用 VSCode）
- 在 docs 目录下编写文章

文件结构为

```
mkdocs.yml
docs/
    index.md
    newfile.md
    xxx/yyy.md
```

- 修改 mkdocs.yml 文件中的 nav 属性 通过缩进可以构造多级目录

例如

```
nav:
  - 首页: index.md
  - 新页面: newfile.md
```

值得注意的是构造多级目录时，缩进应当遵循 yml 语法缩进四个空格

![image-20230101161107381](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202301011611468.png)

有关 MarkDown 、yml 语法可自行百度

MarkDown 文件推荐使用 Typora 编辑

![image-20230101155536007](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202301011555101.png)

VSCode 推荐设置自动保存文件以及保存后自动格式化
