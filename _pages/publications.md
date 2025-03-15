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

<h2>Debug: Show Raw Bibliography Entries</h2>
<pre>{{ site.scholar.bibliography | jsonify }}</pre>

<h2>Single Entry Test: test</h2>
{% bibliography query="@unpublished" limit=1 %}

<h2>Manually Calling One Entry</h2>
{% bibliography query="test" %}   <!-- Replace with an actual BibTeX key -->
