---
title: Home
layout: home
---

<ul>
    {% for post in site.posts %}
    <li>
        <p>{{post.date | date: "%-d %B %Y"}}</p>
        <h2><a href="{{post.url}}">{{post.title}}</a></h2>
        <div>{{post.date | date: "%-d %B %Y"}}</div>
        {{post.excerpt}}
    </li>
    {% endfor %}
</ul>