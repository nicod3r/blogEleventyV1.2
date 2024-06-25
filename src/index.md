---
layout: main.njk
title: texto del título
---

# {{ title }}

Pruebo el contenido de la carpeta con los post correspondiente. 
## tambien agrego contenido extra 
Y en el segundo parrafo agrego {{ title }} lo que considero correspondiente. 

{{ title }}

{% for post in collections.posts %}

- [{{post.data.title}}]({{post.url}})
{{post.data.description}}

{% endfor %}
