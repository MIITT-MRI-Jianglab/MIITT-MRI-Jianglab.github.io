---
title: Conferences
layout: archive
permalink: /conferences/
author_profile: true
---

<ul>
{% assign sorted_conferences = site.data.conferences | sort: 'year' | reverse %}
{% for conference in sorted_conferences %}
<li style="font-size: 16px; margin-bottom: 20px;"> <!-- Added bottom margin -->
   <div style="margin-top: 5px;"> <!-- Added top margin -->
      <em style="font-size: 16px;">{{ conference.authors }}</em> 
      <strong style="font-size: 16px;">{{ conference.title }}</strong>
       
      ,{{ conference.conference }}, {{ conference.year }}, {{ conference.format }} {{ conference.program }}
       {% if conference.award %} <!-- Award display -->
            <span style="
                background-color: #E4D6A0; 
                color: #000; 
                padding: 2px 8px; 
                border-radius: 3px; 
                margin-left: 10px; 
                font-weight: bold;
                font-size: 16px;
            ">{{ conference.award }}</span>
        {% endif %}
       
    
    </div>
    
    
    

        

    
</li>
{% endfor %}
</ul>
