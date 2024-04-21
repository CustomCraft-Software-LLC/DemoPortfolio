---
layout: default
title: Blog
permalink: /blog
---

<div>
    <h1 class="text-center">Blog</h1>

    <ul>
    {% for post in site.posts %}
        <li class="lh-lg">
            <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            <p>{{ post.date | date: "%B %d, %Y" }}</p>
            <p>{{ post.excerpt }}</p>
        </li>
    {% endfor %}
    </ul>
</div>

