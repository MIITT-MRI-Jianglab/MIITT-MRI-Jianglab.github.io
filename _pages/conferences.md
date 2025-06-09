---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

<ul>
{% assign sorted_conferences = site.data.conferences | sort: 'year' | reverse %}
{% for conference in sorted_conferences %}

        {{ conference.authors }}
        {{ conference.title }}
        {{ conference.conference }}, {{ conference.year }},
        {{ conference.format }} {{ conference.program }}
        
        {% if conference.award %} <!-- Award display -->
            <span style="
                font-weight: bold;
            ">{{ conference.award }}</span>
        {% endif %}


</ul>
