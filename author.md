---
layout: page
title: Author
description: A page about the Author
nav_order: 2
---

# Author

{% assign instructor = site.authors%}
{% for author in instructor %}
{{ author }}
{% endfor %}


