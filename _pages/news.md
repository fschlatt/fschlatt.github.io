---
layout: page
title: News
permalink: /news/
description: A collection of news and announcements.
nav: true
nav_order: 4
horizontal: false
---

<div class="news">
{% if site.news != blank -%}
{%- assign news_size = site.news | size -%}
<div class="table-responsive" {% if include.limit and site.announcements.scrollable and news_size > 3 %}style="max-height: 60vw"{% endif %}>
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%}
    {% if include.limit and site.announcements.limit %}
    {% assign news_limit = site.announcements.limit %}
    {% else %}
    {% assign news_limit = news_size %}
    {% endif %}
    {% for item in news %}
    <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
        {% if item.inline -%}
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
        {%- else -%}
            <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
        {%- endif %}
        </td>
    </tr>
    {%- endfor %}
    </table>
</div>
{%- else -%}
<p>No news so far...</p>
{%- endif %}
</div>