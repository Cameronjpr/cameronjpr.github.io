---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
{%- if site.posts.size > 0 -%}
<ul class="posts">
	{%- for post in site.posts -%}
	<li class="post-container">
		{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
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
