# Jamstack Themes

A list of themes and starters for the Jamstack and static site generators. https://jamstackthemes.dev

## 새로운 Taxonomy (필터)를 추가하고싶을 때 거쳐야하는 일
1. content 폴더 밑에 새로운 폴더를 추가 (taxonomy의 이름으로)
2. 그리고 config.toml에 taxonomy hierarchy 추가
3. 각각 md 파일에 해당 taxonomy 파라미터를 추가
4. filters.html에 해당 taxonomy filter를 노출시킴
5. theme-card.html에 해당 taxonomy range를 추가


## Submit A Theme

Anyone can submit an open-source theme by doing a pull request.

1. Fork this repo and create a new markdown `.md` file in `content/theme` folder. For example `hugo-air.md`. 
2. Add the required front-matter as shown in the **Example Theme** below.
3. Submit a pull request

> 💡 Another option is to add a new file using the [Github UI](https://github.com/stackbit/jamstackthemes/tree/master/content/theme) _(click the "add file" button)_ 

**Example Theme**
```yaml
---
title: "My Theme Name"
github: https://github.com/username/repo
demo: https://www.demo.com 
author: authorname
date: 2019-08-20
ssg:
  - Gridsome
cms:
  - No CMS
css:
  - Bootstrap 
archetype:
  - Blog
  - Portfolio
description: This is an amazing theme and this is a small description about it!
---

# A simple starter kit for Gridsome

This theme is a lightweight starter kit. It also gives you a well organised starting point to extend it for yourself.

## Features

* Customisable design tokens to make it your own  
* Customisable global data and navigation  
* Tags and tag archives  
* Progressively enhanced, semantic and accessible  
```

    
## Submission Guidelines

* Any open source themes with a public github repo can be submitted.
* Please make sure the `demo` links to a theme demo and not your personal/business site. The demo url must use https
* at least 1 `ssg` is required.
* at least 1 `cms` is required. If your theme uses markdown (no CMS) the cms should be "No CMS"
