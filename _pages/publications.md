---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---



{% include base_path %}



<ol>
  {% for post in site.publications %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ol>

