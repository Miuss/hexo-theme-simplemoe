# SimpleMoe
[HEXO](https://hexo.io/) 简单萌萌的中文主题😵

![预览图](https://ww2.sinaimg.cn/large/005zWjpngy1fobop9gdt5j311y0lc0vo.jpg)
----------

> 一个不标准的Hexo主题

本主题制作灵感来自于 [@卜卜口](http://mouto.org)

## 功能
本主题主页可编辑个人介绍，页面可以分类显示文章，有独特的相册文章页面。

## 演示
[在线演示](http://miuss.github.io)

## 安装

```bash
git clone https://github.com/Miuss/hexo-theme-simplemoe.git themes/simplemoe
```

## 配置
在这里介绍如何使用本主题（[SimpleMoe](https://github.com/miuss/hexo-theme-SimpleMeo)）

### `Config.yml` （config）

#### Site

```
title: 谬蜀黍
author: 谬蜀黍
```
#### URL

```
url: http://www.miuss.org
root: /
permalink: c/:category/:title/
```

#### Directory

```
category_dir: c
```
#### Themes

```
theme: simplemoe
```

### `Config.yml` （theme.config）

#### 导航

```
menu:
  谬蜀黍: /
  代码: /c/code
  相册: /c/photos
  后感: /c/feel
  链接: /links 
```

#### 个人信息

```
authorimg: 头像链接
autograph: 个人签名
codec: 代码分类页面下方的签名
photosc: 相册分类页面下方的签名
feelc: 后感分类页面下方的签名
```

#### Gitment评论
详细配置请看: 

[https://imsun.net/posts/gitment-introduction/ ](https://imsun.net/posts/gitment-introduction/ )

#### 链接
链接配置就不用嗦了...

## 写作

修改预设文件 `/scaffolds/post.md`

```
---
title: {{ title }}
date: {{ date }}
categories: 
bgimg: 
imgs: 
---
```

写作分类代码ID如下:

- 代码 `code`
- 相册 `photos`	
- 后感 `feel`

> 然后 `bgimg` 和 `imgs` 只有在写相册分类的文章时再做编辑，如果编写其他文章就可以不需要编写。

## 其他

这里详细介绍其他页面的配置方法。

### 链接

在 `/source` 建立 `links/index.md` 文件还有 `/_data/links.yml` 文件。

`links/index.md` 文件内容

```
---
title: 链接
layout: links
---
```

`/_data/links.yml` 文件内容

```
名字:
  link: 链接
  avatar: 头像
  desc: 介绍
```

### 版权问题

本主题可以二次开发但必须标注原作者版权信息，版权信息显示在审查元素中。

添加版权标签方法如下：

```javascript
console.log('\n %c ヾ(≧∇≦)〃SimpleMoe 二次开发版权证明 %c @名字<网址> 年份/月期/日期 \n\n','color:#484848;background:#ffffff;padding:5px 0;', 'color:#ffffff;background:#484848;padding:5px 0;');
	/*这行注释的意义在于，愿看到代码的能保留上面一行 OAQ */
```
