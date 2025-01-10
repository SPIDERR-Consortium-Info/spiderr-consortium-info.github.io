---
permalink: /tools/
title: "Tools"
layout: archive
excerpt: "Tools created for the SPIDeRR research project"
author_profile: true
redirect_from: 
  - /tools.html
  - /tools
---

{% include base_path %}

<style>
  div {
    max-height: 400px; 
    min-height: 200px
  }

  img {
    max-height: 200px;
    width: auto;
  }
</style>

{% for tool in site.tools reversed %} 
  {% include archive-single-tool.html %} 
  <hr>
{% endfor %}
