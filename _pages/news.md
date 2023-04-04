---
layout: page
permalink: /news
title: news
nav: news
---

<div class="table-responsive">
    <table class="table table-sm table-borderless">
        {% assign sorted_news = site.data.news | sort: "date" | reverse %}
        {% for item in sorted_news %}
            <tr>
                <th scope="row" style="font-size: 1rem">{{ item.date | date: "%b %Y" }}</th>
                <td style="font-size: 1rem">{{ item.content | markdownify }}</td>
            </tr>
        {%- endfor %}
    </table>
</div>
