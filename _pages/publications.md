---
layout: page
permalink: /publications/
title: publications
description: My publications in reverse chronological order.
years: [2019, 2018, 2017, 2016, 2015, 2014, 2013]
---





add icons https://iconmonstr.com/
Author names first last.

<h3 class="year">Preprints</h3>
{% bibliography -f preprints %}

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
