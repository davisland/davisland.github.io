---
layout: post
permalink: /blog/
---
<h1 class="headline">Davislog</h1><br>
{% for post in site.categories.drafts %}   
<h2><a href="{{post.url | prepend: site.baseurl}}">{{post.title}}</a></h2>
<h4>{{ post.date | date: "%B %-d, %Y" }}</h4>
{{ post.excerpt }}
{% endfor %}