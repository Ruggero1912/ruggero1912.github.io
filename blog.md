<ul style="margin-left:0; list-style:none;">
  {% for post in site.posts %}
    <li>
          <a class="post-title h-entry u-url" href="{{ post.url }}">{{ post.title }}</a>
        <span class="post-meta"> <span>{{ post.date | date: "%-d %B %Y" }}</span>
         |
         <!-- This is a work around to content | reading_time which does not work on github pages because custom plugins are not allowed --> 
          {% capture words %}
          {{ post.content | number_of_words | minus: 180 }}
          {% endcapture %}
          {% unless words contains '-' %}
          {{ words | plus: 180 | divided_by: 180 | append: ' minutes to read' }}
          {% endunless %}
         </span>
        <br>
        <span class="post-excert">
        {{ post.excerpt }} 
          
            <!-- < a href="{ { post.u rl } }" >... read more< / a > -->

        </span>
    </li>
  {% endfor %}
</ul>