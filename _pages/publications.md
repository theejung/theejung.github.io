---
layout: page
permalink: /publications/
title: publications
description: Conducted projects in study and works.
years: [Nov - Dec 2016, 2015, 2014, 2013]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

