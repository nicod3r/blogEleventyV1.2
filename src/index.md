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
            <article>
                <h2><a href="{{ post.url }}">{{ post.data.title }}</a></h2>
                <p>{{ post.data.description }}</p>
                <small>{{ post.data.fecha }}</small>
            </article>
        {% endfor %}
