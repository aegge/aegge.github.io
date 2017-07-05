---
layout: archive
permalink: /presentations/
author_profile: false
---

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.categories.presentation %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% include presentation-single.html %}
{% endfor %}
