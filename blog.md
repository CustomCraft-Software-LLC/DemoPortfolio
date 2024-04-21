---
layout: default
title: Blog
permalink: /blog
---

<div>
    <h1 class="text-center">Blog</h1>

    <ul class="list-group list-group-flush">
    {% for post in site.posts %}
        <li class="lh-lg list-group-item">
            <h2><a class="link-underline-light" href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            <p>{{ post.date | date: "%B %d, %Y" }}</p>
        </li>
    {% endfor %}
    </ul>
</div>

