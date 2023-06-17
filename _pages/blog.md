---
layout: home-blog
title: "Blog"
permalink: /blog/
lang: fr
classes: wide
authors : true
entries_layout: grid
header: 
#   overlay_color: "#000"
intro: 
  - excerpt: "Ce blog est notre contribution au débat au sein de notre activité"
---

{%- for post in site.tags[include.taxonomy] -%}
  {%- unless post.hidden -%}
    {% include archive-single.html %}
  {%- endunless -%}
{%- endfor -%}