---
title: "Past Editions"
permalink: /editions/
---

# Past Editions

{% for e in site.data.editions %}{% unless e.status == "upcoming" %}
### DMR {{ e.year }} — {{ e.ordinal }} International Workshop on Designing Meaning Representations

{% if e.note %}{{ e.note }}<br>{% endif %}
{{ e.date }}{% if e.location %} &middot; {{ e.location }}{% endif %}{% if e.colocated %} &middot; co-located with {{ e.colocated }}{% endif %}

{% if e.url %}[Workshop website]({{ e.url | relative_url }}){% if e.proceedings %} &middot; {% endif %}{% endif %}{% if e.proceedings %}[Proceedings in the ACL Anthology]({{ e.proceedings }}){% endif %}
{% endunless %}{% endfor %}

---

No workshop was held in 2022. The 2021 edition was organized jointly with the 15th Linguistic Annotation
Workshop and its papers appear in the combined LAW–DMR proceedings.
