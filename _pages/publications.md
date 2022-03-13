---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022,2021,2018]
nav: true
---

Below you can find a list of my publications, with supplementary resources. Please [contact me](mailto:micheli.ferla@gmail.com) if some data is missing.

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
