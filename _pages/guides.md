---
layout: page
title: Side Hustle Guides
permalink: /guides/
---

# Side Hustle Guides

Step-by-step guides for building real side income with AI tools.

These aren't theory — they're the exact workflows we use ourselves.

---

## Available Guides

{% for post in site.posts %}
  {% if post.category == "guide" %}
- **{{ post.title }}** — *{{ post.date | date: "%B %d, %Y" }}*
  {% endif %}
{% endfor %}

---

*More guides added weekly. [Subscribe to updates →](/subscribe/)*