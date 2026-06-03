# 邢介政个人简历项目

这是基于 `D:\jianli\syt-nju.github.io-master` 参考项目整理出的个人简历站点，保留 Minimal Mistakes / academicpages 风格的左侧作者栏、顶部导航和正文排版。

## 内容来源

- 简历文本来源：`C:/Users/DELL/xwechat_files/wxid_1ad2wq54e37p12_0e05/msg/file/2026-06/jxtrue(1).pdf`
- 图片来源：`D:\jianli\资料`
- 站点骨架来源：`D:\jianli\syt-nju.github.io-master`

没有在 PDF 中出现的信息均保留为 `***`，不补写未经确认的学校、账号、论文、专利、项目仓库或导师信息。

## 页面结构

- `/`：主页概览
- `/experience/`：实习与工作经历
- `/projects/`：项目拆解
- `/background/`：教育、技能、课程、竞赛和待补充信息

## 常用文件

- `_config.yml`：站点标题、作者信息、邮箱、电话、头像等全局配置
- `_data/navigation.yml`：顶部导航
- `_pages/about.md`：主页
- `_pages/experience.md`：经历页
- `_pages/projects.md`：项目页
- `_pages/cv.md`：背景页
- `images/`：头像、校徽和组织 logo
- `assets/css/main.scss`：主题样式和少量简历专用样式

## 本地运行

该项目是 Jekyll 站点。安装 Ruby 和 Bundler 后，在项目目录运行：

```bash
bundle install
bundle exec jekyll serve
```

然后访问 `http://localhost:4000`。
