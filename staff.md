---
layout: page
title: Staff
permalink: /staff/
---

We are blessed to have many awesome volunteers....here are a few of them!

{% for personb in site.data.people %}
{% assign person = personb[1] %}
{% if person.bio %}
<div class="card">
    <img class="card-img-top" src="{{ site.url }}/images/people/{{ person.img }}" alt="{{ person.name }}">
    <div class="card-body">
        {% if person.name %}<h5 class="card-title">{{ person.name }}</h5>{% endif %}
        {% if person.email %}<p class="card-text"><small class="text-muted"><a href="mailto:{{ person.email }}">{{ person.email }}</a></small></p>{% endif %}
        {% if person.bio %}<p class="card-text">{{ include person.bio }}</p>{% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
