---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

<!-- {% include base_path %} -->
<!-- <p> Journal Articles </p>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->

<!--<ul>{% for post in site._publicationsJournals reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  -->

  <ul>{% for post in site._publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>