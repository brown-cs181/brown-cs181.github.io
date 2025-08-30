---
layout: default
title: Staff
windowTitle: STAFF
icon: star.png
link_types: []
links: []
---

<!-- # {{ page.title }} -->

<!-- <!-- ### Professor and HTA -->

<!-- <div class="uta-container">
  {% assign professors = site.staff | where: 'role', 'Professor' %}
  {% for staffer in professors %}
  {{ staffer }}
  {% endfor %}
</div>

{% assign HTAs = site.staff | where: 'role', 'HTA' %}
{% if HTAs.size != 0 %}

<div class="uta-container">
  {% for staffer in HTAs %}
  {{ staffer }}
  {% endfor %}
  {% endif %}
</div> -->

<!-- {% assign STAs = site.staff | where: 'role', 'STA' %}
{% if STAs.size != 0 %} --> -->
<!-- 
### STAs

<div class="uta-container">
  {% for staffer in STAs %}
  {{ staffer }}
  {% endfor %}
  {% endif %}
</div> -->

<!-- {% assign STAFF = site.staff | where: 'role', 'staff' %}
{% if STAFF.size != 0 %} -->

<!-- ### UTAs -->

<!-- <div class="uta-container">
  {% for staffer in STAFF %}
  {{ staffer }}
  {% endfor %}
  {% endif %}
</div> -->

<div class="uta-container">
  <!-- First: Professors -->
  {% assign professors = site.staff | where: 'role', 'Professor' %}
  {% for staffer in professors %}
  {{ staffer }}
  {% endfor %}
  
  <!-- Second: HTAs -->
  {% assign HTAs = site.staff | where: 'role', 'HTA' %}
  {% for staffer in HTAs %}
  {{ staffer }}
  {% endfor %}
  
  <!-- Third: UTAs -->
  {% assign UTAs = site.staff | where: 'role', 'UTA' %}
  {% for staffer in UTAs %}
  {{ staffer }}
  {% endfor %}
</div>
