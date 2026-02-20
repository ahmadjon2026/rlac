---
title: "Responses"
permalink: /responses/
layout: archive
author_profile: true
---


{% for post in site.categories.responses %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %d, %Y" }}</small>

{{ post.excerpt }}

---
{% endfor %}