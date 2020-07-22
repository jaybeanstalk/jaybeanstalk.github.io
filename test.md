---
layout: page
title: Staff Members
permalink: /staff/
---
{% for staff-member in site.staff-members %}
  <h2>
    <a href="{{ staff-member.url }}">
      {{ staff-member.name }} - {{ staff-member.position }}
    </a>
  </h2>
  <p>{{ staff-member.content | markdownify }}</p>
{% endfor %}

