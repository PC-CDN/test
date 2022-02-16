---
permalink: index.html
---
{% assign font_files = site.static_files | where: "fobt", true %}
 {% for myimage in font_files %}
 {{ myimage.path }}
{% endfor %}
