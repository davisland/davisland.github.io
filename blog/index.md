---
layout: default
title: blog
permalink: /blog/
---

<ul class="post-list">
	{% for post in site.posts %}
		<li>
			<h1><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1><br><a href="{{ post.url }}">{{ post.date | date: "%b %-d, %Y" }}</a><br><br>
			{{ post.content | strip_html | truncatewords:75}} <br><br>
		</li>
			{% endfor %}
</ul>

<br>

<p class="rss-subscribe">subscribe <a href="https://itunes.apple.com/us/podcast/audio-blog/id1014815356">via iTunes</a> for audio</p>