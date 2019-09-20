<h1 align="center"><a href="https://github.com/8090lambert/hexo-theme-easy">hexo-theme-easy</a></h1>

`hexo-theme-easy` 一款让你爱不释手的优雅、高度配置化，简单易用的 `hexo` 主题，个人博客也在用自己，嘻嘻，欢迎 star~ 
> 参考 **[aero-dual](https://github.com/levblanc/hexo-theme-aero-dual)**，集成其他定制的东西。 它是快速建立你的博客，开始享受它吧！ 

![](https://raw.githubusercontent.com/8090Lambert/material/master/preview.jpg)

**[Demo here](http://8090lambert.cn)**

## Feature
截止到目前为止，主题内集成了下列这些功能，都是即插即用，可以根据自己的需求来。
- 评论系统
    - [Disqus](https://wordpress.org/plugins/disqus-comment-system/) 
    - [Gitalk](https://github.com/gitalk/gitalk)
    - [Gitment](https://github.com/imsun/gitment)
    - [Hypercomments](https://www.hypercomments.com/)
    - [Valine](https://leancloud.cn/)
- 统计 & 分析
    - [Google](https://analytics.google.com/analytics/web/#/report-home/a146263529w208108969p200684717)
    - [Baidu](https://tongji.baidu.com/web/welcome/login)
    - Sougou
    - CNZZ
- 文章封面图
- 代码块高亮
- 个性化页脚定义
- 定制化`menu`
- 全站 pv 统计
- 首页的文章`metadata`定制

## 安装
```
$ cd hexo (hexo main directory)
$ git clone https://github.com/8090lambert/hexo-theme-easy.git themes/easy
```

## 配置文件
```
$ vi themes/easy/_config.yml
```

### 菜单
集成了 `font-awesome`，在菜单可以选择 `文本` 和 `Icon`:
```
# Header Menu
menu:
  Home: /
  Archives: /archives
  Email: mailto:<juzs215@gmail.com>
  # change github values to your own addresses
  Github:
    url: https://github.com/8090Lambert
    icon: github
```

### 首页封面图
```
# URL of the Home page image, For example:
# index_cover: /img/default-banner.jpg
# index_cover: http://8090lambert.cn/img/default-banner.jpg
index_cover: /img/default-banner.jpg
```

### 文章摘要
默认 200 字
```
# Use post content to trim portion text.
auto_excerpt:
  enable: true 
  length: 200   # trim length, default 200
```

### 文章 MetaData
依赖`hexo-wordcount`，需要提前安装：
`
$ cd hexo_dict && npm install hexo-wordcount --save
`
```
# Post meta display settings
post_meta:
  item_text: true
  created_at: true
  updated_at: true
  categories: true

# Post wordcount display settings
# Dependencies: https://github.com/willin/hexo-wordcount
post_wordcount:
  item_text: true
  wordcount: true
  min2read: false
  totalcount: false
  separated_meta: true
```

### 评论系统
选择一个要使用的平台，申请对应的 appid & appkey (不允许同时开启多个)
```
# Many Comment Drivers, you can choose one to open it.
# Write your configure of which platform.

# disqus
disqus_shortname: false

# uyan
uyan_uid: false

# Gitment，https://github.com/imsun/gitment
gitment:
  enable: false
  owner: 
  repo: 
  client_id: 
  client_secret: 

# Gitalk,
gitalk:
  enable: false
  owner: 
  repo: 
  admin: 
  client_id: 
  client_secret: 

# Valine Comment system. https://valine.js.org
valine:
  enable: false
  appId:  # your leancloud appId
  appKey:  # your leancloud appKey
  notify: false # Mail notify
  verify: false # Verify code
  avatar: mm # Gravatar style : mm/identicon/monsterid/wavatar/retro/hide
  placeholder: Just go go # Comment Box placeholder
  guest_info: nick,mail,link # Comment header info
  pageSize: 10 # comment list page size

# Hyper Comments support. Write your id here, or false to disable. http://hypercomments.com
hyper_id: false
```

### 页脚
```
# Footer setting.
footer:
  # Specify the date when the site was setup.
  # If not defined, current year will be used.
  since: 2016

  # Icon between year and copyright info.
  icon: heart

  # If not defined, will be used `author` from Hexo main config.
  copyright: 8090Lambert

  # Hexo link (Powered by Hexo).
  powered: false
```

### 全站 PV 统计
```
# Show PV/UV of the website/page with busuanzi.
# Get more information on http://ibruce.info/2015/04/04/busuanzi/
busuanzi_count:
  # count values only if the other configs are false
  enable: true
```

### 统计 & 分析
根据自己需要去开启，可以同时启用多个
```
# Google Analytics Write your tracking id here, or false to disable.s
google_analytics: 
google_site_verification: 

# CNZZ
cnzz: false

# BaiDu Analytics
baidu_tongji: false

# Sougou Verification.
sogou_site_verification: false
```
