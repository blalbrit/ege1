---
layout: page
show_title: false
banner:
  collection: liturgical
  pid: ege1_stanford
  y: 25%
---

Ege Manuscript 1


---

## Browse Exhibits

<ul>
	{% for item in site.exhibits %}
		{% if item.layout == "exhibit" %}
		<li><a href="{{ site.baseurl }}{{ item.permalink }}">{{ item.title }}</a></li>
		{% endif %}
	{% endfor %}
</ul>

---

## Browse Images

{% include collection_gallery.html collection="liturgical" facet_by="tag" %}

---

## Learn More

<ul>
	{% for item in site.exhibits %}
		{% if item.layout != "exhibit" and item.title != "Browse..." %}
		<li><a href="{{ site.baseurl }}{{ item.permalink }}">{{ item.title }}</a></li>
		{% endif %}
	{% endfor %}
</ul>
