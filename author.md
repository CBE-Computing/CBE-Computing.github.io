---
layout: page
title: Author
description: A page about the Author
---

# Author
Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Instructors

{% assign authors = site.author | where: 'role', 'Emeritus CBE IT' %}
{% for author in authors %}
{{ author }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ author }}
{% endfor %}
{% endif %}
