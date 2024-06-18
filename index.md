---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
seo:
  type: Course
  name: Just the Class
---

# Introduction to Computational Thinking with Data &#x1f4ca;

{: .mb-2 }
UC Berkeley, Summer 2024
{: .mb-2 .fs-6 .text-grey-dk-000 }

{: .mb-2 }
**Instructors:** Atticus Ginsborg, Edwin Vargas Navarro
{: .mb-0 .fs-5 .text-grey-dk-000 }
<!--{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
<div class="role">
  {% for staffer in instructors %}
  {{ staffer }}
  {% endfor %}
</div>-->

## Announcements

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}

{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign active-mods = '' | split: '' %}

{% for mod in mods %}
  {% if mod.status == 'Active' %}
    {% assign active-mods = active-mods | push: mod %}
  {% endif %}
{% endfor %}

{% for module in site.modules %}
{{ module }}
{% endfor %}
