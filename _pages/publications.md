---
title: Publications
layout: page
permalink: /publications/
---

{% raw %}{% assign publications = site.data.publications | sort: "year" | reverse %}
{% assign journals = publications | where: "type", "article" %}
{% assign conferences = publications | where: "type", "inproceedings" %}
{% assign books = publications | where: "type", "book" %}

## Journal Articles
{% for pub in journals %}
<div class="publication">
  <strong>{{ pub.title }}</strong><br>
  {{ pub.author }}<br>
  <em>{{ pub.journal }}</em>, {{ pub.year }}{% if pub.volume %}, {{ pub.volume }}{% endif %}{% if pub.pages %}:{{ pub.pages }}{% endif %}<br>
  {% if pub.doi %}[<a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>]{% endif %}
  {% if pub.url %}[<a href="{{ pub.url }}" target="_blank">PDF</a>]{% endif %}
</div>
{% endfor %}

## Conference Papers
{% for pub in conferences %}
<div class="publication">
  <strong>{{ pub.title }}</strong><br>
  {{ pub.author }}<br>
  <em>{{ pub.booktitle }}</em>, {{ pub.year }}{% if pub.pages %}, pp. {{ pub.pages }}{% endif %}<br>
  {% if pub.doi %}[<a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>]{% endif %}
  {% if pub.url %}[<a href="{{ pub.url }}" target="_blank">PDF</a>]{% endif %}
</div>
{% endfor %}

## Books
{% for pub in books %}
<div class="publication">
  <strong>{{ pub.title }}</strong><br>
  {{ pub.author }}<br>
  <em>{{ pub.publisher }}</em>, {{ pub.year }}<br>
  {% if pub.doi %}[<a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>]{% endif %}
  {% if pub.url %}[<a href="{{ pub.url }}" target="_blank">PDF</a>]{% endif %}
</div>
{% endfor %}

<style>
.publication {
  margin-bottom: 25px;
  padding-bottom: 15px;
  border-bottom: 1px solid #eee;
}
.publication strong {
  font-size: 1.1em;
  color: #1a0dab;
}
.publication em {
  color: #006621;
}
.publication a {
  margin-right: 8px;
  font-family: monospace;
}
</style>{% endraw %}
