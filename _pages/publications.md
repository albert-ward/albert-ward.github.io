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

<h2>Publications</h2>
<div class="publications">
  {% bibliography bib="papers" template="bib_entry"%}
</div>

<br><br>

<h2>Working Papers</h2>
<div class="publications">
  {% bibliography bib="working_papers" template="bib_entry"%}
</div>

{% bibliography papers %}

{% bibliography working_papers %}

<h2>Debug Output</h2>
<p>Bibliography List: {{ site.scholar.bibliography_list }}</p>

<h2>Single Entry Test</h2>

<h3>Papers</h3>
{% bibliography bib="papers" query="@article" %}

<h3>Working Papers</h3>
{% bibliography bib="working_papers" query="@unpublished" %}
