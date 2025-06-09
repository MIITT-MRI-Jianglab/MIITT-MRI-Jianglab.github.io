---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

{% assign sorted_conferences = site.data.conferences | sort: 'year' | reverse %}
{% for conference in sorted_conferences %}

<div style="margin-bottom: 20px; padding-bottom: 15px; border-bottom: 1px solid #eee;">
    <div style="margin-bottom: 5px;">
        <span style="font-style: italic;">{{ conference.authors }}</span>
    </div>
    
    <div style="margin-bottom: 5px;">
        <strong style="font-size: 16px;">{{ conference.title }}</strong>
        {% if conference.award %} 
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
    </div>
    
    <div>
        <span>{{ conference.conference }}</span>, 
        <span>{{ conference.year }}</span>,
        <span>{{ conference.format }}</span>
        {% if conference.program %}
            <span> • {{ conference.program }}</span>
        {% endif %}
    </div>
</div>
