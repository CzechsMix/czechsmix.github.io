---
layout: page
title: Blog
permalink: /blog/
---
{% for post in site.posts %}
### {{post.title}}
{% for tag in post.tags %}<span class="tag {{tag}}">{{tag}}</span>{% endfor %}
{{post.excerpt}}
<span class="more">[Read More...]({{post.url}})</span>
{% endfor %}
