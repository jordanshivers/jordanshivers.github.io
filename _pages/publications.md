---
layout: page
permalink: /publications/
title: publications
description: 
years: [2023,2022,2021,2020,2019,2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md --> 

via <a href="https://scholar.google.com/citations?user=mAHTjjoAAAAJ"><b>Google Scholar</b></a>
<br>
via <a href="https://orcid.org/0000-0002-3884-1708"><b>ORCID</b></a> 
<br>
via <a href="https://jordanshivers.github.io/assets/pdf/cv.pdf"><b>my CV</b></a> <br>


<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
