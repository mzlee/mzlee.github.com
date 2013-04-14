---
layout: page
title: Some guy's blog
tagline: Systems and security in CS
---
{% include JB/setup %}

## Posts

{% for post in site.posts %}
  <div>
    <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a><br />
	<span class="blurb">{{ post.content | strip_html | truncatewords:25 }}</span>
  </div>
{% endfor %}
