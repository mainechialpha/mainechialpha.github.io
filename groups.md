---
layout: connect
title: Discipleship Groups
permalink: /groups/
---

![Discipleship Groups]({{ site.url }}/images/d-group.jpg)

In a Discipleship Group (D-Group), you're going to meet real people. Ones who talk about their struggles in the moment. You'll learn what trust can look like--not because you've known each other for forever, but because your leaders will lead in transparency, because there's a mutual entrusting, because you're with people who are being truly present. It's a place to process and ask questions and share victories. You don't need to know what you think about everything to participate. You'll fight next to each other, but you'll also fight for each other--if something needs to be prayed about, you'll pray for it right then. In a D-Group, prayer is an action. You'll see brother and sisterhood in action as you seek and fight for truth together. You'll always ask the question, "now that I know, what am I going to do about it?" This is the difference between a Bible study and a D-Group, because we believe if we know truth, our life needs to be defined by it. We're not reading through the Word so we can say we know what it says, but because this is the manual and we need to apply it in every place it's usable.

Here are our current offerings for Fall 2021! To get connected with a leader, scroll to the bottom of this page & fill out the google form. We can't wait to meet you!

## Men's D-Groups

{% for groupb in site.data.mensdgroups %}
{% assign group = groupb[1] %}
{% if group.name %}

<div class="d-sm-flex align-items-sm-center flex-sm-row shadow-card card">
    <img class="group-img col-5" src="{{ site.url }}/images/mensdgroups/{{ group.img }}" alt="{{ group.name }}">
    <div class="group-body">
        {% if group.name %}<h5 class="group-title">{{ group.name }}</h5>{% endif %}
        {% if group.time %}<p class="group-time"><small class="text-muted">{{ group.time }}</small>{% endif %}</p>
    </div>
</div>
{% endif %}
{% endfor %}

## Women's D-Groups

{% for groupb in site.data.womensdgroups %}
{% assign group = groupb[1] %}
{% if group.name %}

<div class="d-sm-flex align-items-sm-center flex-sm-row shadow-card card">
    <img class="group-img col-5" src="{{ site.url }}/images/womensdgroups/{{ group.img }}" alt="{{ group.name }}">
    <div class="group-body">
        {% if group.name %}<h5 class="group-title">{{ group.name }}</h5>{% endif %}
        {% if group.time %}<p class="group-time"><small class="text-muted">{{ group.time }}</small>{% endif %}</p>
    </div>
</div>
{% endif %}
{% endfor %}

<p style="text-align: center;"><a href="https://forms.gle/P22icC57cftW8GQ87" class="btn btn-primary my-1">Connect to a D-Group leader here!</a></p>
