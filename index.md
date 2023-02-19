---
title: Home
layout: home
---

<ul>
    {% for post in site.posts %}
    <li>
        <h2><a href="{{post.url}}">{{post.title}}</a></h2>
        <div>Posted by {{post.author}} on {{post.date | date: "%-d %B %Y"}}</div>
        {%if post.brief%}
            <p><em>{{post.brief}}</em></p>
        {% else %}
        {{post.excerpt}}
        {%endif%}

    </li>
    {% endfor %}
</ul>