### Posts

<ul style="margin-left:0; list-style:none;">
  {% for post in site.posts %}
    <li>
        <div class="feed-post-container">
          {% if post.image %}
              
              <img src="{{ post.image }}" alt="{{post.title}}" class="feed-post-image"  />
              
          {% endif %}
        <div>
          <a class="post-title h-entry u-url" href="{{ post.url }}">{{ post.title }}</a>
          <br/>
        <span class="post-meta"> <span>{{ post.date | date: "%-d %B %Y" }}</span>
         |
         <!-- This is a work around to content | reading_time which does not work on github pages because custom plugins are not allowed --> 
          {% capture words %}
          {{ post.content | number_of_words | minus: 180 }}
          {% endcapture %}
          {% if words contains '-' %}
          1 minute to read
          {%else %}
          {{ words | plus: 180 | divided_by: 180 | append: ' minutes to read' }}
          {% endif %}
         |
         Posted by
          {% if post.author %}
          {{ post.author }}
          {% else %}
          {{ site.author }}
          {% endif %}
         </span>
        <br>
        <span class="post-excert">
        {{ post.excerpt | strip_html | truncatewords: 15 }} 
          
            <a href="{{ post.url }}"> read more</a>

        </span>
        </div>
        </div>
    </li>
  {% endfor %}
</ul>