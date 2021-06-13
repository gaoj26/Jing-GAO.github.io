---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



<head>
<style>
a:visited {
  color: grey;
  background-color: transparent;
  text-decoration: none;
}
a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}
</style>
</head>

<body>

<ol>
  {% for post in site.publications reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <a href="{{post.paperurl}}">[Download]</a>
    </li>
  {% endfor %}
</ol>

</body>
