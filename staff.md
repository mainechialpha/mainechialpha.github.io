---
layout: about
title: Staff
permalink: /staff/
---

We are blessed to have many awesome volunteers....here are a few of them!

{% for personb in site.data.people %}
{% assign person = personb[1] %}
{% if person.bio %}
<div class="shadow-card card">
    <img class="person-img col-3" src="{{ site.url }}/images/people/{{ person.img }}" alt="{{ person.name }}">
    <div class="person-body">
        {% if person.name %}<h5 class="person-title">{{ person.name }}</h5>{% endif %}
        {% if person.email %}<p class="person-email"><small class="text-muted"><a href="mailto:{{ person.email }}">{{ person.email }}</a></small></p>{% endif %}
        {% if person.bio %}<p class="person-text">{{ person.bio }}</p>{% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
