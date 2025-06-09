---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

<ul>
{% assign sorted_conferences = site.data.conferences | sort: 'year' | reverse %}
{% for conference in sorted_conferences %}
    <div>
        {{ conference.authors }}
        {{ conference.title }}
        {{ conference.journal }}, {{ conference.year }}
        {{ conference.format }} {{ conference.program }}
        
        {% if conference.award %} <!-- Award display -->
            <span style="
                background-color: #ffd700; 
                color: #000; 
                padding: 2px 8px; 
                border-radius: 3px; 
                margin-left: 10px; 
                font-weight: bold;
                font-size: 14px;
            ">{{ conference.award }}</span>
        {% endif %}
  
</li>
{% endfor %}
</ul>
