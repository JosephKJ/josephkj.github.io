---
layout: page
permalink: /publications/
title: Publications
description: 4 x CVPR, 2 x ICCV, 2 x ECCV, 2 x WACV, 1 x {TPAMI, NeurIPS, AAAI, IJCAI, BMVC, IROS}
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
