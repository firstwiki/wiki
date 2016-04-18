---
layout: page
title: People of FIRST
permalink: /people
---

{% assign items = site.people | sort: 'title' %}
{% for doc in items %}{% if doc.url != page.url %}* [{{ doc.title}}]({{ site.baseurl }}{{ doc.url }}){% endif %}
{% endfor %}
