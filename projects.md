### My Projects

<ul style="margin-left:0; list-style:none;">
  {% for project in site.projects %}
    <li>
          <a class="post-title h-entry u-url" href="{{ project.url }}">{{ project.name }}</a>
        <span class="post-meta"> <span>{{ project.date | date: "%B %Y" }}</span>
         |
         <!-- This is a work around to content | reading_time which does not work on github pages because custom plugins are not allowed --> 
          {% capture words %}
          {{ project.content | number_of_words | minus: 180 }}
          {% endcapture %}
          {% if words contains '-' %}
          1 minute to read
          {%else %}
          {{ words | plus: 180 | divided_by: 180 | append: ' minutes to read' }}
          {% endif %}
         |
         Posted by
          {{ site.author }}
         </span>
        <br>
        <span class="post-excert">
        {{ project.excerpt | strip_html | truncatewords: 15 }} 

            <a href="{{ project.url }}" >... read more</a>

        </span>
    </li>
  {% endfor %}
</ul>