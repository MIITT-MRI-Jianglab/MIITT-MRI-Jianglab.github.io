---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

<ul>
{% assign sorted_conferences = site.data.conferences | sort: 'year' | reverse | group_by: 'year' %}

{% for year_group in sorted_conferences %}
    {% assign conferences_in_year = year_group.items | sort: 'program' %}
    
    {% for conference in conferences_in_year %}
    <li style="font-size: 14px; margin-bottom: 16px;">
        <div style="margin-top: 5px;">
            <em>{{ conference.authors }}</em> 
            <strong>{{ conference.title }}</strong>,
            
            {% if conference.location %}
                {{ conference.conference }} ({{ conference.location }}), 
            {% else %}
                {{ conference.conference }}, 
            {% endif %}
            
            {{ conference.year }}, {{ conference.format }} {{ conference.program }}
            
            {% if conference.award %}
                <span style="
                    background-color: #E4D6A0;
                    color: #000;
                    padding: 2px 4px;
                    border-radius: 2px;
                    margin-left: 5px;
                    font-weight: bold;
                    display: inline-block;
                    margin-top: 2px;
                ">{{ conference.award }}</span>
            {% endif %}
        </div>
    </li>
    {% endfor %}
{% endfor %}
</ul>
