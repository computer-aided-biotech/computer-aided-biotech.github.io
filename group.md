---
layout: page
title: The Team
permalink: /group/
---

<!-- <div class="card-deck">
    maybe use later
</div> -->

{% for person in site.people %}
<div class="card" style="width: 18rem;">
  <img class="card-img-top" src="{{ person.image_url }}" alt="Card image cap">
  <div class="card-body">
    {% if person.linkedin %}
        <a href="https://www.linkedin.com/in/{{ person.linkedin }}/"><i class="bi bi-linkedin"></i></a>
    {% endif %}
    {% if person.twitter %}
        <a href="https://www.twitter.com/{{ person.twitter }}/"><i class="bi bi-twitter"></i></a>
    {% endif %}
    <p class="card-text">{{ person.excerpt }}</p>
  </div>
</div>
{% endfor %}


## Alumni

{% for person in site.alumni %}
<div class="card" style="width: 18rem;">
  <img class="card-img-top" src="{{ person.image_url }}" alt="Card image cap">
  <div class="card-body">
    {% if person.linkedin %}
        <a href="https://www.linkedin.com/in/{{ person.linkedin }}/"><i class="bi bi-linkedin"></i></a>
    {% endif %}
    {% if person.twitter %}
        <a href="https://www.twitter.com/{{ person.twitter }}/"><i class="bi bi-twitter"></i></a>
    {% endif %}
    <p class="card-text">{{ person.excerpt }}</p>
  </div>
</div>
{% endfor %}


