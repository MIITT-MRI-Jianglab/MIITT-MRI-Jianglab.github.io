
---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


# Academic Publications

{% raw %}{% assign pubs = site.data.publications | sort: "year" | reverse %}
{% assign articles = pubs | where: "type", "article" %}
{% assign conferences = pubs | where: "type", "inproceedings" %}
{% assign books = pubs | where: "type", "book" %}

## Journal Articles
{% for pub in articles %}
<div class="pub-item">
  <div class="pub-title">{{ pub.title }}</div>
  <div class="pub-authors">{{ pub.authors }}</div>
  <div class="pub-venue">
    <em>{{ pub.journal }}</em>
    {% if pub.volume %}, Vol. {{ pub.volume }}{% endif %}
    {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
    ({{ pub.year }})
  </div>
  <div class="pub-links">
    {% if pub.doi %}
    <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
    {% endif %}
    {% if pub.url %}
    <a href="{{ pub.url }}" target="_blank">PDF</a>
    {% endif %}
  </div>
</div>
{% endfor %}

## Conference Papers
{% for pub in conferences %}
<div class="pub-item">
  <div class="pub-title">{{ pub.title }}</div>
  <div class="pub-authors">{{ pub.authors }}</div>
  <div class="pub-venue">
    <em>{{ pub.booktitle }}</em>
    {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
    ({{ pub.year }})
  </div>
  <div class="pub-links">
    {% if pub.doi %}
    <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
    {% endif %}
    {% if pub.url %}
    <a href="{{ pub.url }}" target="_blank">PDF</a>
    {% endif %}
  </div>
</div>
{% endfor %}

## Books
{% for pub in books %}
<div class="pub-item">
  <div class="pub-title">{{ pub.title }}</div>
  <div class="pub-authors">{{ pub.authors }}</div>
  <div class="pub-venue">
    <em>{{ pub.publisher }}</em> ({{ pub.year }})
  </div>
  <div class="pub-links">
    {% if pub.doi %}
    <a href="https://doi.org/{{ pub.doi }}" target="_blank">DOI</a>
    {% endif %}
    {% if pub.url %}
    <a href="{{ pub.url }}" target="_blank">PDF</a>
    {% endif %}
  </div>
</div>
{% endfor %}

<style>
.pub-item {
  margin-bottom: 1.8rem;
  padding-bottom: 1.2rem;
  border-bottom: 1px solid #eaeaea;
}
.pub-title {
  font-weight: 600;
  font-size: 1.1rem;
  margin-bottom: 0.3rem;
  color: #1a0dab;
}
.pub-authors {
  font-size: 0.95rem;
  color: #555;
  margin-bottom: 0.3rem;
}
.pub-venue {
  font-size: 0.9rem;
  margin-bottom: 0.4rem;
}
.pub-links a {
  display: inline-block;
  margin-right: 12px;
  padding: 3px 10px;
  background: #f1f8ff;
  border: 1px solid #c8e1ff;
  border-radius: 3px;
  color: #0366d6;
  text-decoration: none;
  font-size: 0.85rem;
}
.pub-links a:hover {
  background: #def;
}
</style>{% endraw %}
  You can find my articles on [Google Scholar](https://scholar.google.com/citations?user=IgJsqoIAAAAJ&hl=en&authuser=1).

  
{% include base_path %}
