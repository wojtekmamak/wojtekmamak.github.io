---
layout: archive
title: "Popular Writing"
permalink: /popular/
author_profile: true
---

Here you'll find my non-academic writing—essays, blog posts, and articles aimed at broader audiences interested in philosophy, cognitive science, and the history of ideas.

{% include base_path %}

{% for post in site.popular reversed %}
  {% include archive-single.html %}
{% endfor %}
