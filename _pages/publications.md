---
title: Publications
layout: archive
permalink: /publications/
author_profile: true
---
# Publications

{% for publication in site.data.publications %}
**{{ publication.title }}**  
   *{{ publication.authors }}*  
   Published in {{ publication.journal }}, {{ publication.year }}  
   [Read more]({{ publication.url }})
{% endfor %}
