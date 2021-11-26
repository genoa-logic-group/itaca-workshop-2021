---
title: Programme 
permalink: /programme/

layout: page
---

|------------------------| 
| **Monday 20 December**     | 
|------------------------|
| 13.30 - 15.00 | slot 1 |
| 15.00 - 15.30 | break  |
| 15.30 - 17.00 | slot 2 |
| 17.00 - 17.30 | break  |
| 17.30 - 18.30 | slot 3 |
|------------------------| 
| **Tuesday 21 December**    |
|------------------------| 
| 09.00 - 10.30 | slot 4 | 
| 10.30 - 11.00 | break  | 
| 11.00 - 12.30 | slot 5 | 
| 12.30 - 14.00 | break  | 
| 14.00 - 15.30 | slot 6 | 
|------------------------| 

## Speakers 

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
