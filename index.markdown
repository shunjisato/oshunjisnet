---
layout: home
title: "Portfolio"
---

# Works

<div class="works-gallery">
  {%- for page in site.pages -%}
    {%- if page.path contains "work/" -%}
    <div class="work-item">
      <a href="{{ page.url | relative_url }}">
        <img src="{{ page.thumbnail | relative_url }}" alt="{{ page.title }}">
        <h3>{{ page.title }}</h3>
      </a>
      <p>{{ page.excerpt }}</p>
    </div>
    {%- endif -%}
  {%- endfor -%}
</div>
