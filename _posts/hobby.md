---
title: Foo Bar
layout: tag
permalink: /hobby/
---
<ul class="tags">

	{% for tag in page.tags %}
		
		<li><a href="/tags#{{ tag }}" class="tag">{{ tag }}</a></li>

		{% for post in site.tags.tag %}

			<ul class="taglinks">

				<li><a href="{{ post.url }}">{{ post.title }}</a></li>

			</ul>

		{% endfor %}

	{% endfor %}
</ul>
