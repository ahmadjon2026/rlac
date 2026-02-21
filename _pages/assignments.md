---
title: "Assignments"
layout: archive
permalink: /assignments/
author_profile: true


---

{% assign posts = site.categories.assignments %}
{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}