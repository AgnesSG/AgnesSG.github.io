---
layout: page
permalink: /publications/
title: Publications
description: Peer-reviewed publications, theses and conference contributions
years: [2021, 2015, 2013, 2012, 2010, 2006, 2001]
nav: true
---

<div class="publications">

  {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f papers -q @*[year={{y}}]* %}
  {% endfor %}

</div>
