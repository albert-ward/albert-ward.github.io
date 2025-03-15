---
layout: page
permalink: /publications/
title: research
description: publications and working papers in reverse chronological order.
nav: true
nav_order: 2
scholar:
  bibliography: _bibliography/papers.bib
  bibliography_list:
    papers: _bibliography/papers.bib
    working_papers: _bibliography/working_papers.bib
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<h2>Publications</h2>
<div class="publications">
  {% bibliography bib="papers.bib" template="bib_entry" %}
</div>

<br><br>
<br><br>

<h2>Working Papers</h2>
<div class="working_papers">
  {% bibliography bib="working_papers.bib" template="bib_entry" %}
</div>
