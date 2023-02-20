---
layout: page
title: Publications
permalink: /publications/
description: star(*) denotes equal contribution
years: [2023, 2022, 2021, 2020, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
