---
layout: post
title: All post
description: Tat ca san pham.
image: assets/images/banner-02.jpg
nav-menu: true
---

<!-- All post -->

<div class="inner">
{% for post in site.posts %}
{% if post.type == 'san-pham' %}
{% if post.title != 404 %}
	<p>
	<a href="{{site.baseurl}}{{post.url}}" >
		<h2>{{ post.title }}</h2>
	</a>
	<!-- {% if post.image %}<span class="image main"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></span>{% endif %} -->
	<br>{% if post.date %} {{ post.date }} {% endif %}
	<br><h3>{{ post.description }}</h3>
	</p>
{% endif %}
{% endif %}
{% endfor %}
</div>
