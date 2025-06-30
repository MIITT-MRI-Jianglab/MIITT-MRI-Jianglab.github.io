---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

<ul>
{% assign confs_by_year = site.data.conferences | group_by: 'year' %}
{% assign years_sorted = confs_by_year | sort: 'name' | reverse %}

{% for year in years_sorted %}
    {% comment %} Create a temporary array with numerical program values {% endcomment %}
    {% assign confs_with_num = '' | split: '' %}
    {% for conf in year.items %}
        {% assign new_conf = conf %}
        
        {% comment %} Convert program number to integer {% endcomment %}
        {% assign num = conf.program | plus: 0 %}
        
        {% comment %} Create a temporary sort_num property {% endcomment %}
        {% assign new_conf = new_conf | hash: 'sort_num', num %}
        {% assign confs_with_num = confs_with_num | push: new_conf %}
    {% endfor %}
    
    {% comment %} Sort by the temporary sort_num property numerically {% endcomment %}
    {% assign sorted_confs_in_year = confs_with_num | sort: 'sort_num' %}
    
    {% for conference in sorted_confs_in_year %}
    <li style="font-size: 14px; margin-bottom: 20px;">
        <div style="margin-top: 5px;">
            <em>{{ conference.authors }}</em> 
            <strong>{{ conference.title }}</strong>,<br>
            
            {% if conference.location %}
                {{ conference.conference }} ({{ conference.location }}), 
            {% else %}
                {{ conference.conference }}, 
            {% endif %}
            
            {{ conference.year }}, {{ conference.format }} 
            
            {% comment %} Display original program value exactly as in YAML {% endcomment %}
            {{ conference.program }}
            
            {% if conference.award %}
                <span style="
                    background-color: #E4D6A0;
                    color: #000;
                    padding: 2px 8px;
                    border-radius: 3px;
                    margin-left: 10px;
                    font-weight: bold;
                    display: inline-block;
                    margin-top: 3px;
                ">{{ conference.award }}</span>
            {% endif %}
        </div>
    </li>
    {% endfor %}
{% endfor %}
</ul>
