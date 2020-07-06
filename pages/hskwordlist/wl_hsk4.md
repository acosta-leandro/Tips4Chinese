---
title: HSK 4 (Word List)
keywords: sample
summary: "Hsk 4 - Word List"
sidebar: product1_sidebar
permalink: wl_hsk4.html
folder: hskwordlist
---

<table>
  {% for row in site.data.hskwordlist.hsk4 %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>

<p>These files have been generated from the latest (as of November 2013) which word lists published by Hanban in September 2012</p>
