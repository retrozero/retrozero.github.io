---
layout: bloc-bootstrap_carousel
title: Exemples en images
date:   2021-09-03 13:49:35 +0200
categories: home
lang: fr
---

{% for slide in site.data.btrp_carousel %}

<div class="carousel-item {{ slide.statut }}">
    <img class="d-block w-100" src="{{ slide.img_name }}" alt="{{ slide.alt }}">
    <div class="carousel-caption d-none d-md-block">
        <h5>{{ slide.h5 }}</h5>
        <p> {{ slide.p }} </p>
    </div>
</div>

{% endfor %}
