---
layout: homepage
description: "Apex Renovators"
header-img: "img/frank-robbins-roof.jpg"
---

{% for post in site.posts %}
<div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
        <h2 class="post-title">
            {{ post.title }}
        </h2>
        {% if post.subtitle %}
        <h3 class="post-subtitle">
            {{ post.subtitle }}
        </h3>
        {% endif %}
    </a>
    <p class="post-meta">Posted by {{ post.author }} on {{ post.date | date: "%B %-d, %Y" }}</p>
</div>
<hr>
{% endfor %}
