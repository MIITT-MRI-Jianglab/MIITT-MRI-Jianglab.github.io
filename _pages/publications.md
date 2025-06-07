---
title: Publications
layout: page
permalink: /publications/
---
# My Publications

{% for publication in site.data.publications %}
1. **{{ publication.title }}**  
   *{{ publication.authors }}*  
   Published in {{ publication.journal }}, {{ publication.year }}  
   [Read more]({{ publication.url }})
{% endfor %}
