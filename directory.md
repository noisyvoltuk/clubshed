---
layout: page
title: Directory
permalink: /directory/
---


<ul>
{% for member in site.data.directory %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>