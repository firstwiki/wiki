---
layout: page
title: All wiki pages
---

This is an index of all wiki pages under /wiki/

{% assign items = site.collections | sort: 'label' %}
{% for c in items %}
{% if c.label != "posts" and c.label != "common" %}
### {{ c.label }}
{% assign docs = site[c.label] %}
{% include collection_idx.html collection=docs %}
{% endif %}
{% endfor %}
