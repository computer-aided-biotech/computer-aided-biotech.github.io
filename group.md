---
layout: page
title: The Team
permalink: /group/
---

<div class="card-deck">
    {% for person in site.people %}
    <div class="card">
        <img class="card-img-top" src="{{ person.image_url }}" alt="Card image cap">
        <div class="card-body">
        <h5 class="card-title">{{ person.name}} </h5>
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
</div>

## Alumni


<div class="card-deck">
    {% for person in site.alumni %}
    <div class="card">
        <img class="card-img-top" src="{{ person.image_url }}" alt="Card image cap">
        <div class="card-body">
        <h5 class="card-title">{{ person.name}} </h5>
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
</div>


