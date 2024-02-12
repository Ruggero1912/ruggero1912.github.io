### My Projects

<ul style="margin-left:0; padding-left:0px; list-style:none;">
  {% assign projects = site.projects | sort: "priority" %}
  {% for project in projects %}
    <li>
          <div class="feed-post-container">

          {% if project.image %}
          
          <img src="{{ project.image }}" alt="{{project.name}} logo" class="feed-post-image"  />
          
          {% endif %}

          <div>
          <p><a class="post-title" href="{{ project.url }}">{{ project.name }}:</a> {{ project.short_description }}</p>
            <span class="post-meta"> <span>{{ project.date | date: "%B %Y" }}
            {% if project.active_project %}
            - today 
            {% endif %}
            </span>
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
          </div>
          </div>
    </li>
  {% endfor %}
</ul>