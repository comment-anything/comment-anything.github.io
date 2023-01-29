---
title: Home
layout: home
---

<ul>
    {% for post in site.posts %}
    <li>
        <h2><a href="{{post.url}}">{{post.title}}</a></h2>
        <div>Posted by {{post.author}} on {{post.date | date: "%-d %B %Y"}}</div>
        {{post.excerpt}}
    </li>
    {% endfor %}
</ul>