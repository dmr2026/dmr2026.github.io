---
title: "Designing Meaning Representations"
permalink: /
---

# International Workshop on Designing Meaning Representations

DMR brings together researchers who are producers and consumers of meaning representations. The workshop is a
venue for presenting new frameworks and critically examining existing ones — their design, annotation,
parsing, generation, evaluation, and use in downstream applications — with the goal of informing the design of
next-generation meaning representations. A recurring theme is the relationship between distributed
representations learned by neural models and the symbolic meaning representations designed and annotated by
researchers.

{% assign upcoming = site.data.editions | where: "status", "upcoming" | first %}
{% if upcoming %}
<div class="notice" markdown="1">
### Current edition: [DMR {{ upcoming.year }}]({{ upcoming.url | relative_url }})

**{{ upcoming.ordinal }} International Workshop on Designing Meaning Representations**{% if upcoming.theme %}<br>
*{{ upcoming.theme }}*{% endif %}

Venue and dates: {{ upcoming.date }}. See the [call for papers]({{ upcoming.url | relative_url }}) for the
workshop topic, scope, and organizers.
</div>
{% endif %}

## Editions

| Edition | Workshop | Co-located with | Location | Proceedings |
|:--|:--|:--|:--|:--|
{%- for e in site.data.editions %}
| {{ e.ordinal }} | {% if e.url %}[DMR {{ e.year }}]({{ e.url | relative_url }}){% else %}DMR {{ e.year }}{% endif %} | {{ e.colocated | default: "—" }} | {{ e.location }} | {% if e.proceedings %}[ACL Anthology]({{ e.proceedings }}){% else %}—{% endif %} |
{%- endfor %}

There was no DMR workshop in 2022. Details on each past edition, including the joint LAW–DMR 2021 workshop,
are on the [past editions]({{ '/editions/' | relative_url }}) page.

## Contact

For any questions regarding the workshop, please contact us at
[dmrworkshopofficial@gmail.com](mailto:dmrworkshopofficial@gmail.com), or see the
[DMR {{ upcoming.year }} organizers]({{ '/2027/committees/' | relative_url }}).
