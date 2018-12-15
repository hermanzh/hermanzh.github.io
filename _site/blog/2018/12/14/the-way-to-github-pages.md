[Home](../../../../)

# 今天我的博客开通了 2018-12-14

## 等了好久，终于下定决心开博，想了好久，还是决定用Github Pages，但是苦于自己前端太弱，还是找一个现成的主题，弄了好久才成功，记录一下：

### 创建一个博客
1. 创建一个repo，名称为：your_name.github.io
2. 创建index.html，就是你的博客主页
3. 访问 https://your_name.github.io

### 添加Jekyll主题到你的博客：
1. 在repo中创建一个文件_config.yml，并添加内容
theme: jekyll-theme-[you_choosed_theme]
可用主题见 https://pages.github.com/themes/
2. 根目录下创建Gemfile文件并添加
```
source 'https://gems.ruby-china.com/'
gem "github-pages", group: :jekyll_plugins
```
3. 根目录下创建assets/css/style.scss, 并拷贝

```

---
---

@import "{{ site.theme }}";
```
4. 进入你的repo目录，命令行执行 bundle install, 正确安装gem
5. bundle exec jekyll serve
6. 拷贝https://github.com/pages-themes/THEME_NAME/blob/master/_layouts/default.html（**`THEME_NAME`用你选择的主题名替换**）
到你的目录_layouts/default.html
7. 把index替换成index.md，使用markdown改写
