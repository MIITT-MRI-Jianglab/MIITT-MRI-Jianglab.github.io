---
title: Publications
layout: archive
permalink: /publications/
author_profile: true
---

<ul>
{% assign sorted_publications = site.data.publications | sort: 'year' | reverse %}
{% for publication in sorted_publications %}
<li style="font-size: 14px; margin-bottom: 20px;"> <!-- Added bottom margin -->
    <div>
        <strong style="font-size: 16px;">{{ publication.title }}</strong>
        {% if publication.award %} <!-- Award display -->
            <span style="
                background-color: #ffd700; 
                color: #000; 
                padding: 2px 8px; 
                border-radius: 3px; 
                margin-left: 10px; 
                font-weight: bold;
                font-size: 14px;
            ">{{ publication.award }}</span>
        {% endif %}
    </div>
    <div style="margin-top: 5px;"> <!-- Added top margin -->
        {{ publication.journal }}, {{ publication.year }}<br>
        <em style="font-size: 14px;">{{ publication.authors }}</em><br>
        <!-- <a href="{{ publication.url }}">Read more</a> -->
    </div>
</li>
{% endfor %}
</ul>
