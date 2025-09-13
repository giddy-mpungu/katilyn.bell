---
title: Events
permalink: /events/
layout: page
---

{% for e in site.data.events %}
### {{ e.title }}
**When:** {{ e.date }}  
**Where:** {{ e.location }}

{{ e.description }}

{% if e.registration %}
[Register →]({{ e.registration }})
{% endif %}

---
{% endfor %}
