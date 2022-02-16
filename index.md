---
permalink: index.html
---
{% assign font_files = site.static_files | where: "font", true %}
 {% for myimage in font_files %}
 {{ myimage.path }}
{% endfor %}
