---
layout: page
permalink: /publications/
title: publications
description: 
pre_years: [2023]
pub_years: [2024, 2023,2022,2021,2020,2019,2017]
diss_years: [2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md --> 

via <a href="https://scholar.google.com/citations?user=mAHTjjoAAAAJ"><b>Google Scholar</b></a>
<br>
via <a href="https://orcid.org/0000-0002-3884-1708"><b>ORCID</b></a> 
<br>
via <a href="/cv"><b>my CV</b></a> <br>
<br>

<h3><b>Preprints</b></h3>
<div class="publications">
{%- for y in page.pre_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>
<br>

<h3><b>Peer-reviewed papers</b></h3>
<div class="publications">
{%- for y in page.pub_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
<br>

<h3><b>Dissertation</b></h3>
<div class="publications">
{%- for y in page.diss_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}
</div>