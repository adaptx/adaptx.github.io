---
layout:default
title: 我的Blog
---
<p>{{page.title}}</p>
<p>最新文章</p>
<ul>
    {% for post in site.posts %}
        <li>{{ post.date | date_to_string}}  <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}

</ul>