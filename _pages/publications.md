---
title: Publications
layout: archive
permalink: /publications/
author_profile: true
---

<ul class="publications-list">
{% for publication in site.data.publications %}
<li>
    <strong>{{ publication.title }}</strong><br>
    <em>{{ publication.authors }}</em><br>
    Published in {{ publication.journal }}, {{ publication.year }}<br>
    <a href="{{ publication.url }}">Read more</a>
</li>
{% endfor %}
</ul>

.publications-list li {
    font-size: 14px; /* Customize as desired */
}
