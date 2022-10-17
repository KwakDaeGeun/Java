---
title: "Html"
layout: archive
permalink: /html
author_profile: true
sidebar:                  
        nav: "sidebar-category" 
---


{% assign posts = site.categories.html %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
