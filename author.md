---
layout: page
title: Author
description: A page about the Author
---

# Author

{% assign instructor = site.authors%}
{% for author in instructor %}
{{ author }}
{% endfor %}


