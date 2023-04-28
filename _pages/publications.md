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

<!-- {% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->


## Journals

{% for post in site.publications reversed%}
  {% if post.pubtype == "journal" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Domestic

{% for post in site.publications reversed%}
  {% if post.pubtype == "domestic" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
