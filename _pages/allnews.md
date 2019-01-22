---
title: "BioLab - News"
layout: textlay
excerpt: "BioLab at Sharif University of Technology."
sitemap: false
permalink: /allnews/
---

# News

{% for article in site.data.news %}
  <p>{{ article.date }} <br>
  <em>{{ article.headline }}</em>
    {% if article.image_src %}
      <img src='{{ site.url }}{{ site.baseurl }}{{article.image_src}}' class='img-responsive' style='max-width: 192px' />
    {% endif %}
  </p>
{% endfor %}
