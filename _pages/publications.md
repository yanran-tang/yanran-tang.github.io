---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
\* equal contribution

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>Journal</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Conference</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'conference' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}