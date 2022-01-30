---
layout: default
title: Contributeurs
permalink: /staff
---
# Contributeurs

{% for author in site.authors %}
## [{{ author.name }}]({{ author.url }})
**{{ author.position }}**
<br>
{{ author.content | markdownify }}
<br>
<br>
{% endfor %}

<ul>
  {% for author in site.authors %}
    <li>
      <h2><a href="{{ author.url }}">{{ author.name }}</a></h2>
      <h3>{{ author.position }}</h3>
      <p>{{ author.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>