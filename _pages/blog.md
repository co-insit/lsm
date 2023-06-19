---
layout: home-blog
title: "Blog Natation sauvetage"
permalink: /blog/
lang: fr
classes: wide
authors : true
entries_layout: grid
header: 
#   overlay_color: "#000"
intro: 
  - excerpt: "Ce blog est notre tribune et notre contribution au débat au sein de notre activité. Vous y trouverez des articles techniques, culturels et tous autres contenus dont nous estimons avoir leur place ici. Bonne lecture."
---

{% include feature_row id="intro" type="center" %}

{%- for post in site.tags[include.taxonomy] -%}
  {%- unless post.hidden -%}
    {% include archive-single.html %}
  {%- endunless -%}
{%- endfor -%}