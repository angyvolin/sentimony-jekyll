---
layout: page
title: Artists
description: Artists of Sentimony Records
permalink: /artists/
og-image: https://content.sentimony.com/assets/img/og-images/sentimony/home.jpg
---

{% for i in site.categories.artists reversed %}

{% if i.photo_cover %}
<p>
  <a href="{{ i.url }}">
    <img class="photo-cover" src="{{ i.photo_cover }}" alt="{{ i.title }}">
  </a>
</p>
{% endif %}

{% if i.youtube_id %}
[{{ i.title }}]({{ i.url }})
{% endif %}

{% endfor %}
