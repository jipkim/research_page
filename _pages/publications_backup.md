---
layout: page_book
permalink: /publications_fancy/
title: publications
description: publications by categories in reversed chronological order. 
years: [2022,2021,2020,2019,2017,2016]
nav: true
---
<!-- <img src="/assets/img_page/Bookshelf-unsplash.jpg" width="100%"> -->
<!-- _pages/publications.md -->

<br>
<br>
[Google Scholar](https://scholar.google.com/citations?user=A5c_yfsAAAAJ&hl=en ){: .btn}
[ORCID](https://orcid.org/0000-0002-5185-3631 ){: .btn}

<div class="publications">


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
