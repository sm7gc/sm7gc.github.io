---
layout: page
permalink: /publications
title: publications
nav: publications
description: Check out my <a href="https://scholar.google.com/citations?userid=fZh9riIAAAAJ&user=fZh9riIAAAAJ" target="_blank">Google Scholar</a> for my latest publications
years: [2024,2023, 2021, 2020, 2019, 2018]
---

<!-- <div class="row">
  <label for="journal" class="col-lg-4"><input id="journal" type="checkbox">Journal Articles</label>
  <label for="conference" class="col-lg-4"><input id="conference" type="checkbox">Conference Papers</label>
  <label for="workshop" class="col-lg-4"><input id="workshop" type="checkbox">Workshop Papers</label>
</div> -->

{% for y in page.years %}
  <div class="row m-0 p-0" style="border-top: 1px solid #ddd;">
    <div class="col-sm-1 mt-2 p-0 pr-1">
      <h3 class="bibliography-year col-sm-1 mt-2 p-0 pr-1">{{y}}</h3>
    </div>
    <div class="col-sm-11 p-0">
      {% bibliography -f papers -q @*[year={{y}}]* %}
    </div>
  </div>
{% endfor %}