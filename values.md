---
layout: about
title: Core Values
permalink: /values/
---

<div class="container-fluid">
{% for val in site.data.values %}
{% assign value = val[1] %}
{% if value.body %}
<div class="shadow-card card">
  {% if value.img %}
    <img class="card-img-top" src="{{ site.url }}/images/values/{{ value.img }}" alt="{{ value.title }}">
  {% endif %}
    <div class="card-body">
        {% if value.title %}<h5 class="card-title text-center">{{ value.title }}</h5>{% endif %}
        {% if value.body %}<p class="card-text">{{ value.body }}</p>{% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
</div>
