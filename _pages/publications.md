---
layout: page
permalink: /publications/
title: research
description: publications and working papers in reverse chronological order.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<br><br>

{% assign all_entries = site.scholar.bibliography %}

<h2>Publications</h2>
<ul>
  {% for entry in all_entries %}
    {% if entry.entry_type == "article" or entry.entry_type == "inproceedings" %}
      <li><strong>{{ entry.title }}</strong> ({{ entry.year }}) - {{ entry.journal }}</li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Working Papers</h2>
<ul>
  {% for entry in all_entries %}
    {% if entry.entry_type == "unpublished" %}
      <li><strong>{{ entry.title }}</strong> ({{ entry.year }})</li>
    {% endif %}
  {% endfor %}
</ul>

