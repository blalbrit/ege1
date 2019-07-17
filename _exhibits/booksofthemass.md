---
layout: exhibit
title: "Reconstructing Ege 1"
editor: Benjamin Albritton
publish_date: 2019-07-15
permalink: /exhibits/reconstruction/
---

We mad a reconstruction.

---

## Browse by Image

{% include collection_gallery.html collection="liturgical" facet_by="tag" only="Books of the Mass" %}

---

## Browse by Label

{% for item in site.liturgical %}{% if item.tag == page.title %}
- [{{item.label | remove: 'New York, Columbia University, ' }}]({{site.baseurl}}{{item.permalink}})
{% else %}{% endif %}{% endfor %}

