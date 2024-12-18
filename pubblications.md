### HowTos

<ul style="margin-left:0; list-style:none;">
  {% for post in site.pubblications %}
    <li>
        <div class="feed-post-container">
          {% if post.image %}
              
              <img src="{{ post.image }}" alt="{{post.title}}" class="feed-post-image"  />
              
          {% endif %}
        <div>
          <a class="post-title h-entry u-url" href="{% if post.website %}{{post.website}}{% else %}{{ post.url }}{% endif %}">{{ post.title }}</a>
          <br/>
        <span class="post-meta"> <span>{{ post.date | date: "%-d %B %Y" }}</span>
         |
          {% if post.published_at %}
            published at {{ post.published_at }}
          {% endif %}
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
          
            <a href="{% if post.website %}{{post.website}}{% else %}{{ post.url }}{% endif %}"> read more</a>

        </span>
        </div>
        </div>
    </li>
  {% endfor %}
</ul>