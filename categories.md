---
layout: default
title: Categories
permalink: /categories/
---
{% for category in site.categories %}
  - [{{category | first}}]({{site.url}}{{site.baseurl}}{{page.url}}{{category | first}})
{% endfor %}
