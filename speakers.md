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
**{{ t.title }}**

{% endfor %}
