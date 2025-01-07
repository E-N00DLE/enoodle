---
layout: page
permalink: /text/
title: text
---

<ul class="post-list">
{% for text in site.text reversed %}
    <li>
        <h2><a class="text-title" href="{{ text.url | prepend: site.baseurl }}">{{ text.title }}</a></h2>
        <p class="post-meta">{{ text.date | date: '%Y-%m-%d' }}</p>    
    </li>
{% endfor %}
</ul>
