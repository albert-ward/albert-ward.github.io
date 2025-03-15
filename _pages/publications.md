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

<h2>publications</h2>
<div class="publications">
  {% bibliography query="@article" %}
</div>

<br><br>

<h2>working papers</h2>
<div class="working_papers">
  {% bibliography query="@unpublished" %}
</div>

