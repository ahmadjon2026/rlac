---
title: "Assignments"
layout: archive
permalink: /assignments/
author_profile: true
---

{% for post in site.categories.assignments %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
