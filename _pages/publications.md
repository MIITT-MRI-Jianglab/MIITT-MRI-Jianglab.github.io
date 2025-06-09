---
title: Publications
layout: archive
permalink: /publications/
author_profile: true
---

<ul>
{% assign sorted_publications = site.data.publications | sort: 'year' | reverse %}
{% for publication in sorted_publications %}
<li style="font-size: 14px;"> <!-- Set the size for each list item -->
    <strong style="font-size: 16px;">{{ publication.title }}</strong><br> <!-- Larger size for titles -->
    {{ publication.journal }}, {{ publication.year }}<br>
    <em style="font-size: 14px;">{{ publication.authors }}</em><br>
    <!-- <a href="{{ publication.url }}">Read more</a> -->
</li>
{% endfor %}
</ul>
