---
layout: page
permalink: /text/
title: text
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---

<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%Y-%m-%d' }}</p>    
    </li>
{% endfor %}
</ul>
