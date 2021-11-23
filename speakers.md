---
title: Speakers  
permalink: /speakers/

layout: page
---

{% for t in site.data.talks %}
{% if t.url %}
[{{ t.author }}]({{ t.url }}) ({{ t.affiliation }})  
{% else %}
{{ t.author }} ({{ t.affiliation }})  
{% endif -%}  
**{{ t.title }}** <br/> 
{%- if t.abs %}
[abstract]({{ t.abs | prepend: '/assets/abstracts/' | relative_url }}){:target="_blank"} 
{% endif %}

{% endfor %}
