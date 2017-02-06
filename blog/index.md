---
title: Blog
layout: post
permalink: /blog/
---
<br /><br />
{% for post in site.categories.blog %}   
<h3><a href="{{post.url | prepend: site.baseurl}}">{{post.title}}</a></h3><br>
{% endfor %}