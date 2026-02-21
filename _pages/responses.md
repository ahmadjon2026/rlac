---
title: "Responses"
permalink: /responses/
layout: archive
author_profile: true
---


{% assign posts = site.categories.responses %}
{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}