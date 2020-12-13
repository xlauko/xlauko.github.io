---
layout: page
---


{% for year in (2016..2020) reversed %}

{{ year }}
{% bibliography --query @*[year={{ year }}] %}

{% if forloop.last == false %}
  ---
{% endif %}

{% endfor %}
