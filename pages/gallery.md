---
layout: no-styles
title: Gallery
permalink: /gallery-md/
---

<main class="gallery-wrapper" markdown="1">

# Gallery

{% assign pics = site.static_files | where: "image", true | where_exp: "pic", "pic.path contains 'whiteboard-annotated'" %}

{:.gallery__list}
{% for pic in pics %}
- ![{{ pic.basename }}]({{ pic.path | relative_url }})
  <span>{{ pic.basename }}</span>
{% endfor %}

</main>