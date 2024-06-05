---
layout: page
title: Schedule
description: The weekly event schedule.
---

# Weekly Schedule

Note [SOCS](https://www.berkeley.edu/map/social-sciences-building/) is the Social Sciences Building

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
