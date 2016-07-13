---
layout: default
title: blog
permalink: /blog/
---

<ul class="post-list">
	{% for post in site.posts %}
		<li>
			<h1><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
			<div class="a-mod"><a href="{{ post.url }}">{{ post.date | date: "%b %-d, %Y" }}</a></div><br><br>
			{{ post.summary }} <br><br>
		</li>
			{% endfor %}
</ul>

<p>subscribe <a href="https://itunes.apple.com/us/podcast/audio-blog/id1014815356">via iTunes</a> for audio</p>