---
layout: archive
title: ""
permalink: /publications/
author_profile: true
---

{% include base_path %}

<!-- {% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %} -->


Journal Articles
======
  <ul>{% for post in site.publications reversed %}
  {% if post.category == "Journal Articles" %}
    {% include archive-single-cv.html %}
  {% endif %}
  {% endfor %}</ul>


International Conferences with Proceedings
======
  <ul>{% for post in site.publications reversed %}
  {% if post.category == "International Conferences with Proceedings" %}
    {% include archive-single-cv.html %}
  {% endif %}
  {% endfor %}</ul>

International Conferences without Proceedings
======
  <ul>{% for post in site.publications reversed %}
  {% if post.category == "International Conferences without Proceedings" %}
    {% include archive-single-cv.html %}
  {% endif %}
  {% endfor %}</ul>

National Conferences with Proceedings
======
  <ul>{% for post in site.publications reversed %}
  {% if post.category == "National Conferences" %}
    {% include archive-single-cv.html %}
  {% endif %}
  {% endfor %}</ul>

  
  

<!-- {% for pub in site.publications %}
  {% if pub.category == "Journal Articles" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %} -->




<!-- ul>{% for post in site._publicationsJournals reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  

  <ul>{% for post in site._publications reversed %} 
    {% include archive-single-cv.html %}
  {% endfor %}</ul> 

<ul>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
</ul>  -->

<!-- ## Journal Articles
{% for pub in site.publications %}
  {% if pub.category == "Journal Articles" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %}

## International Conferences with Proceedings
{% for pub in site.publications %}
  {% if pub.category == "International Conferences with Proceedings" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %}

## International Conferences without Proceedings
{% for pub in site.publications %}
  {% if pub.category == "International Conferences without Proceedings" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %}

## National Conferences with Proceedings
{% for pub in site.publications %}
  {% if pub.category == "National Conferences with Proceedings" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %}

## National Conferences without Proceedings
{% for pub in site.publications %}
  {% if pub.category == "National Conferences without Proceedings" %}
    {% include publication.html pub=pub %}
  {% endif %}
{% endfor %} -->


