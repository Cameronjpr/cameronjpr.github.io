---
layout: default
title: Cameron Robson
---

{%- if site.posts.size > 0 -%}

<ul class="posts">
	{%- for post in site.posts -%}
	<li class="post-teaser-container">
		{%- assign date_format = site.date_format | default: "%d-%m-%y" -%}
		<div>
			<a class="post-teaser-title" href="{{ post.url | relative_url }}">
				{{ post.title | escape }}
			</a>
		</div>
		<time class="post-date">{{ post.date | date: date_format }}</time>
	</li>
	{%- endfor -%}
</ul>
{%- endif -%}
