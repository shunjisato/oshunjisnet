---
layout: page
title: "Blog"
permalink: /blog/
---

# Blog

<ul class="blog-list">
  {%- for post in site.posts -%}
  <li>
    <a href="{{ post.url | relative_url }}">
      <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      {{ post.title }}
    </a>
  </li>
  {%- endfor -%}
</ul>
