---
title: Lista de posts
layout: post.njk
---
# {{ title }}

{% for post in collections.posts %}

- [{{post.data.title}}]({{post.url}})
{{post.data.description}}

{% endfor %}