---
layout: default
title: Blog
permalink: /blog/
---

Blog

{% for post in site.posts %}
		<time>{{ post.date | date: "%b %-d, %Y" }}</time>
		<h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
{% endfor %}
