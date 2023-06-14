---
layout: default
title: Portfolio
permalink: /portfolio
---

<ul>
 
  {% for post in site.posts limit: maxposts %}
        <li>
            <p>{{ post.title }}</p>
                <p>
       {{ post.content | strip_html | truncatewords:75 }}
       </p>
            </li>
        {% endfor %}
 
