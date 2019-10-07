---
layout: page
title: publications
permalink: /publications/
description: * denotes equal contribution
years: [2019, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
