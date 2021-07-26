---
layout: page
title: About
description: 程序人生
keywords: Fangting Liu, marsblog, mars的博客
comments: true
menu: 关于
permalink: /about/
---

大家好，我是mars，目前在研究微服务、Docker、K8s、分享开源技术。

坚信熟能生巧，技术改变人生。

业余羽毛球、游戏好者。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
