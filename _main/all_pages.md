---
layout: page
title: All wiki pages
---

This is an index of all wiki pages under /wiki/

{% assign items = site.collections | sort: 'label' %}
{% for c in items %}
{% assign docs = site[c.label] | sort: 'title' %}
{% if c.label != "posts" and c.label != "common" %}
### {{ c.label }}
{% for doc in docs %}{% if doc.layout != 'redirect' %}* [{{ doc.title }}]({{ site.baseurl }}{{ doc.url }}) {% endif %}
{% endfor %}
{% endif %}
{% endfor %}
