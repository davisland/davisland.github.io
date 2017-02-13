---
layout: post
permalink: /blog/
---
<h1 class="headline">Blog</h1>
{% for post in site.categories.blog %}   
<h3><a href="{{post.url | prepend: site.baseurl}}">{{post.title}}</a></h3><br>
{% endfor %}