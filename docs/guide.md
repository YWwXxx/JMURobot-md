# 集美大学机器人创新实验室博客上传方式

## 网址

1. 首先了解一下实验室官网地址(http://www.jmurobot.com)，<u>官网仅仅作为实验室展示页面，用于展示实验室简介、实验室团队成员介绍、图片展示、项目展示。</u>
2. 其次了解一下实验室博客地址(https://jmurobot-md.readthedocs.io/en/latest/)，该网站用于团队成员写博客、描述项目等。

## 修改实验室官网展示内容方式

- 输入 url(http://www.jmurobot.com/wp-admin)`账号：JMURobot 密码：**\***` (登录可能会等待一段时间)

![image-20230224155256820](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241552101.png)

- 左侧菜单栏-->外观-->自定义

![image-20230224155956094](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241559151.png)

- 点击后进入编辑页面

![image-20230224160032829](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241600865.png)

- 这里我们举例修改照片区域

下划到想要修改的部分(**在可修改的地方会出现铅笔的图标**)

![image-20230224160245308](/Users/yeweixin/Library/Application Support/typora-user-images/image-20230224160245308.png)

- 点击铅笔图标

![image-20230224160434704](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241604740.png)

- 选择图片页面

![image-20230224160742630](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241607696.png)

- 确认无误后，<strong style="color:red">点击发布</strong>，等待一会后即可完成内容的修改

![image-20230224160852084](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241608131.png)

> 文字修改也类似，在 WordPress 中还有很多可供修改的地方，比如文字可以用 css 定义样式等等，可自行百度。

## 上传博客方式

### 前提

⚠️<strong style="color:red">上传博客需要使用 Git，如果不会 Git 也不用担心，可在[Gitee][https://gitee.com]官网查看教程以及获取相关工具</strong>![gitee-img](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241615538.png)

### 步骤

- 第一步要先拉取 git 仓库的代码，地址为(https://github.com/YWwXxx/JMURobot-md.git)

采用指令`git clone https://github.com/YWwXxx/JMURobot-md.git`，在想要拉取的位置 调用**命令行**输入、回车即可(拉取的时间可能比较久)。无法使用 git 指令的自行百度，在这里不再赘述。

![image-20230224162216095](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241622154.png)

- 拉取完成后 用 VSCode 打开(推荐在 VSCode 中配置 git 插件，方便提交拉取)

![image-20230224163258869](https://ywwxxx.oss-cn-fuzhou.aliyuncs.com/markdown/202302241632931.png)

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

​ ⚠️<strong style="color:red">希望各位能规范 Git 提交，在提交前设置 Git 全局的 Username 和 Email；在提交时备注提交信息 commit，如“本次由某某某提交了 xxx 项目记录”；清晰提交记录</strong>
