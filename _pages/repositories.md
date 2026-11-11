---
layout: page
permalink: /repositories/
title: repositories
description: 
nav: true
nav_order: 4
---

{% assign repos = site.github.public_repositories | where: "fork", false | sort: "created_at" | reverse %}

{% if repos.size > 0 %}

## github repositories
<br>
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in repos %}
    {% unless site.data.repositories.repo_exclude contains repo.name %}
      {% include repository/repo.liquid repository=repo.full_name description=repo.description %}
    {% endunless %}
  {% endfor %}
</div>
{% endif %}
