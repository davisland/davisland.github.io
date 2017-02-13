---
layout: post
permalink: /blog/
---
<h1 class="headline">Blog</h1><br><br>
{% for post in site.categories.drafts %}   
<h3><a href="{{post.url | prepend: site.baseurl}}">{{post.title}}</a></h3><br>
{% endfor %}