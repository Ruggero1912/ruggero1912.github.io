<ul style="margin-left:0; list-style:none;">
  {% for post in site.posts %}
    <li>
        <h2>
          <a class="post-title h-entry u-url" href="{{ post.url }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta"> <span>{{ post.date | date: "%-d %B %Y" }}</span> | {{ post.content | reading_time }}</span>
        <br>
        <span class="post-excert">
        {{ post.excerpt }} 
          
          <a href="{{ post.url }}">... read more</a></span>
    </li>
  {% endfor %}
</ul>