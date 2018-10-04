---
layout: plain
title: Gallery
permalink: /gallery/
---

# Gallery

{% assign pics = site.static_files | where: "image", true | where_exp: "pic", "pic.path contains 'whiteboard-annotated'" %}

{% for pic in pics %}
- ![{{ pic.basename }}]({{ pic.path | relative_url }})
{% endfor %}