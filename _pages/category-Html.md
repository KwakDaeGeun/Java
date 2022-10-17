---
title: "blog"
layout: archive
permalink: /html
---


{% assign posts = site.categories.Html %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
