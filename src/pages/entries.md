---
title: "All Entries"
description: "Stuff I wrote on here"
---
<div class="irevamp-section slide-up">
<ul class="irevamp-list-unstyled">
      {%- for page in collections.entry | reverse -%}
        <li class="irevamp-postlist">
          <div class="irevamp-postlist__content">
            <a href="{{ page.url }}" class="irevamp-text">{{ page.data.title }}</a>
            <p class="irevamp-lead">{{ page.data.date | postDate  }} {% if page.data.description %} • {{ page.data.description }}</p>{% endif %}
          </div>
        </li>
      {%- endfor -%}
</ul>
</div>