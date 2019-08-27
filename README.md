<h1 align="center"><a href="https://github.com/8090lambert/hexo-easy-theme">hexo-easy-theme</a></h1>

<p align="center">hexo-easy-theme is a high quality elegant <a href="http://hexo.io">Hexo</a> theme.</p>
 
This theme build on **[aero-dual](https://github.com/levblanc/hexo-theme-aero-dual)**, and it integrated other Customization things. It is make for quickly building you blog, enjoy it!

**[Demo here](http://8090lambert.cn)**

## Features
- Comments system
    - Disqus
    - Gitalk
    - Gitment
    - Hypercomments
    - UYan
    - Valine
- Analytics and Statistics
    - Google
    - Baidu
    - Sougou
    - CNZZ
- Image cover for post page
- Highlight syntax for code block
- Customization footer for you
- Text and icon for menu
- Pv statistics with busuanzi

## Install
```
$ git clone https://github.com/8090lambert/hexo-easy-theme.git themes/easy
```
> Note: Please let you Hexo version great than or equal to 3.2

## Usage
Set theme in main **hexo config** `_config.yml` file:
```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: easy
```

## Preview
You can use command `hexo server` to start a local server see your change.

## Configuration
These configuration options in theme `_config.yml` file，unless special illustration.

### Menu
This menu support `text` or `icon(font-awesome)`, for example:
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

### Home Cover Image
```
# URL of the Home page image, For example:
# index_cover: /img/default-banner.jpg
# index_cover: http://8090lambert.cn/img/default-banner.jpg
index_cover: /img/default-banner.jpg
```

### Auto excerpt
```
# Use post content to trim portion text.
auto_excerpt:
  enable: true 
  length: 200   # trim length, default 200
```

### Post MetaData
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

### Comments
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

### Custom Footer
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

### PV Statistics
```
# Show PV/UV of the website/page with busuanzi.
# Get more information on http://ibruce.info/2015/04/04/busuanzi/
busuanzi_count:
  # count values only if the other configs are false
  enable: true
```

### Analytics
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

## License

MIT
