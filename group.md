---
layout: page
title: Group
permalink: /group/
---

{% for person in site.people %}
<li>
    <img class="picture" src="{{ person.image_url }}" {{ person.name}} >
</li>
{% endfor %}

## Allumni