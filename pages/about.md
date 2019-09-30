---
layout: page
title: 关于
description: 记录软件人生
keywords: hui-Zz, 咖辉
comments: true
menu: 关于
permalink: /about/
---

我是咖辉，永远追求一劳永逸的解决方案！

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
