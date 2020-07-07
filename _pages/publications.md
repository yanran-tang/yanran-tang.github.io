---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
\* equal contribution

You can also find my articles on <u><a href="https://scholar.google.com/citations?user=zbRZyuEAAAAJ&hl=en">my Google Scholar profile</a>.</u>

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