---
layout: page
permalink: /publications/
title: publications
# description: publications by categories in reversed chronological order. generated by jekyll-scholar.
years: [2019, 2021, 2022, 2023, 2024, 2025]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{%- for y in page.years reversed %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
