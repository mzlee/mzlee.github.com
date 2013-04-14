---
layout: page
title: Trying something new...
tagline: Systems and security in CS
---
{% include JB/setup %}

## Posts

{% for post in site.posts %}
  <div>
    <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
	<span>{{ post.content | strip_html | truncatewords:50 }}</span>
  </div>
{% endfor %}
