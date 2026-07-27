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


<!-- ## Publications -->

<style>
/* Slightly tighter line spacing for Publications (font size unchanged) */
.publications-list .list__item { margin-bottom: 1.4em; }
/* Align image top with title top (theme adds a top margin to the image) */
.publications-list .content-image { margin-top: 0; }
.publications-list .archive__item-title { font-size: 1.1em; line-height: 1.25; margin: 0 0 0.25em; }
.publications-list .archive__item-excerpt { font-size: 0.95em; line-height: 1.35; margin: 0.3em 0; }
.publications-list .content-details > p { font-size: 0.95em; line-height: 1.35; margin: 0.3em 0; }
</style>

<div class="publications-list">
{% for post in site.publications reversed%}
  {% if post.pubtype == "publications" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
</div>

<!-- ## Conference Papers

{% for post in site.publications reversed%}
  {% if post.pubtype == "conference" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %} -->