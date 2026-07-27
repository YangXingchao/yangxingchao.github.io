---
layout: archive
title: "Misc"
permalink: /misc/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<!-- {% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->


<!-- ## Papers -->

<style>
/* Misc is less prominent than Publications: smaller type, tighter spacing */
.misc-list .list__item { margin-bottom: 0.9em; }
.misc-list .archive__item-title {
  font-size: 1rem;
  line-height: 1.25;
  margin: 0.2em 0 0.15em;
}
.misc-list .archive__item-excerpt {
  font-size: 0.8rem;
  line-height: 1.3;
  margin: 0.15em 0;
}
.misc-list .content-details > p {
  font-size: 0.8rem;
  line-height: 1.3;
  margin: 0.15em 0;
}
</style>

<div class="misc-list">
{% for post in site.misc reversed%}
  {% if post.pubtype == "domestic" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
</div>
