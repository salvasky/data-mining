---
layout: default
---

# My GitHub Page

Welcome to my GitHub Page! Check out these files:

{% for file in site.github.repository.files %}
  {% if file.path != 'index.md' %}
    - [{{ file.name }}]({{ file.path }})
  {% endif %}
{% endfor %}
