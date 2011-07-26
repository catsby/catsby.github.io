---
layout: archive
permalink: archive.html
title: Archive
category: archive
published: true
---

<ul>
{% for post in site.posts %}
    {% unless post.type == 'page' %}
        <li><a href="{{post.url}}">{{post.title}}</a><span class="post-date-archive">{{post.date | date_to_string}} </span></li>
    {% endunless %}
{% endfor %}
</ul>