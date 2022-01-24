---
layout: home
title: HOME
image: /images/3OpS_logo300px.png
---

<ul class="list3">
    {% for category in site.categories %} {%- if category[0] == "events" -%}
    {%- for post in category[1] -%}
    <li class="list3__item">
        <div class="box--3">
            <a href="{{ post.url }}">
            <img src="{{ post.image }}">
            </a>
        </div>
    </li>
    {%- endfor -%}
    {%- endif -%} {% endfor %}
<ul>
