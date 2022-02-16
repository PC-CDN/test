---
permalink: index.html
---
{% assign font_files = site.static_files | where: "font", true %}
 {% for myfontfiles in font_files %}
 {{ myfontfiles.path }}
     {.% if myfontfiles.extname == 'ttf' %}
         <li>{{ myfontfiles.url }}</li>
         <li>{{ myfontfiles.basename }}</li>
         <li>{{ myfontfiles.name }}</li>
         <li>{{ myfontfiles.extname }}</li>
         <li></li>
         <li></li>
         <li></li>
         <li></li>
     {.% endif %}

{% endfor %}
