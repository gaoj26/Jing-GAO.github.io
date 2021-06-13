---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!--{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->



<!--{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}-->

{% include base_path %}

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

<h2>Journal</h2>

<ol>
  {% for post in site.publications reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <a href="{{post.paperurl}}">[Download]</a>
    </li>
  {% endfor %}
</ol>

<h2>Conference</h2>
<ol>
  {% for post in site.talks reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <a href="{{post.paperurl}}">[Download]</a>
    </li>
  {% endfor %}
</ol>

</body>
