---
layout: post-project
title: Nội thất
description: Một số dự án đã tham gia triển khai.
image: assets/images/banner-01.jpg
nav-menu: true
---
<section id="photos">
<div class="row-no-gutters">
    {% for post in site.posts %}
	{% if post.type == 'project' %}
	<div class="img_wrap">
		{% if post.image %}
		<a href="{{site.baseurl}}{{post.url}}" class="portfolio-box">
		  <img src="{{site.baseurl}}/assets/images/thumbs/{{ post.image }}" class="image" >	
		</a>
		<p class="img_description">{{post.description}}</p>
		{% endif %}
	</div>
   {% endif %}
   {% endfor %}
</div>
</div>

<!-- <script src="{{site.baseurl}}/js/photo-grid.js"></script> -->
<script>
function getRandomSize(min, max) {
  return Math.round(Math.random() * (max - min) + min);
}
</script>
