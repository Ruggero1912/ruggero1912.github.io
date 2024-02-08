# Welcome to My Portfolio! 🚀

## About Me ℹ️
I am a passionate software engineer currently pursuing my Master's degree in Artificial Intelligence and Data Engineering at the University of Pisa, following my Bachelor's degree in Computer Engineering from the same institution. 

With a strong foundation in software engineering, coupled with expertise in deep learning, cloud computing, and data engineering, I am dedicated to leveraging technology to solve complex problems and drive innovation.

## Projects 💻

### Coming soon 🖼️
- **Description:** 
- **Technologies Used:** 
- **Link:** 

### Project 2 ☁️

### Project 3 📊


## Blog 📝

### Latest Articles 📰

<ul style="margin-left:0; list-style:none;">
  {% for post in site.posts limit:3 %}
    <li>
          <a class="post-title h-entry u-url" href="{{ post.url }}">{{ post.title }}</a>
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
         </span>
        <br>
    </li>
  {% endfor %}
</ul>

Visit the [blog](/blog) section for the complete list of articles.

## Education 🎓
- **Master's Degree:** Artificial Intelligence and Data Engineering, University of Pisa (Expected Graduation: MM/YYYY)
- **Bachelor's Degree:** Computer Engineering, University of Pisa (04/2021)

## Contact Me 📬
Feel free to reach out to me via email at [giacomo@paciosoft.com](mailto:giacomo@paciosoft.com) or connect with me on [LinkedIn](https://dronesimulator.it/r/my-linkedin).