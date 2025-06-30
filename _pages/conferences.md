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
                {% comment %} Determine award color based on award type {% endcomment %}
                {% assign award_type = conference.award | downcase %}
                {% assign award_color = "#E4D6A0" %} {% comment %} Default gold color {% endcomment %}
                
                {% if award_type contains "summa" %}
                    {% assign award_color = "#FFD700" %} {% comment %} Gold - Summa Cum Laude {% endcomment %}
                {% elsif award_type contains "magna" %}
                    {% assign award_color = "#C0C0C0" %} {% comment %} Silver - Magna Cum Laude {% endcomment %}
                {% elsif award_type contains "cum laude" %}
                    {% assign award_color = "#CD7F32" %} {% comment %} Bronze - Other Cum Laude {% endcomment %}
                {% endif %}
                
                <span style="
                    background-color: {{ award_color }};
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
