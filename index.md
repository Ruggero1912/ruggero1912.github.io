# 👋 Hi! I'm Giacomo Pacini

## About Me ℹ️
I am a passionate software engineer currently pursuing my Master's degree in Artificial Intelligence and Data Engineering at the University of Pisa, following my Bachelor's degree in Computer Engineering from the same institution. 

With a strong foundation in software engineering, coupled with expertise in deep learning, cloud computing, and data engineering, I am dedicated to leveraging technology to solve complex problems and drive innovation.

## Projects 💻

### dronesimulator 🚁📝🔎
- **Description:** I developed a web platform that simulates the exam needed to achieve the Open Category UAS pilot certificate (drone pilot), it currently has **more than 21.000 users**.
It implements also machine learning techniques for questions classification.
- **Technologies Used:** PHP, SQL, APIs, JavaScript, Python, Flask, SciKit Learn
- **Link:** [dronesimulator.it](https://dronesimulator.it) 

### Mobile (<svg role="img" viewBox="0 0 24 24" width=24 height =24 xmlns="http://www.w3.org/2000/svg"><title>Android</title><path fill="#34A853" d="M18.4395 5.5586c-.675 1.1664-1.352 2.3318-2.0274 3.498-.0366-.0155-.0742-.0286-.1113-.043-1.8249-.6957-3.484-.8-4.42-.787-1.8551.0185-3.3544.4643-4.2597.8203-.084-.1494-1.7526-3.021-2.0215-3.4864a1.1451 1.1451 0 0 0-.1406-.1914c-.3312-.364-.9054-.4859-1.379-.203-.475.282-.7136.9361-.3886 1.5019 1.9466 3.3696-.0966-.2158 1.9473 3.3593.0172.031-.4946.2642-1.3926 1.0177C2.8987 12.176.452 14.772 0 18.9902h24c-.119-1.1108-.3686-2.099-.7461-3.0683-.7438-1.9118-1.8435-3.2928-2.7402-4.1836a12.1048 12.1048 0 0 0-2.1309-1.6875c.6594-1.122 1.312-2.2559 1.9649-3.3848.2077-.3615.1886-.7956-.0079-1.1191a1.1001 1.1001 0 0 0-.8515-.5332c-.5225-.0536-.9392.3128-1.0488.5449zm-.0391 8.461c.3944.5926.324 1.3306-.1563 1.6503-.4799.3197-1.188.0985-1.582-.4941-.3944-.5927-.324-1.3307.1563-1.6504.4727-.315 1.1812-.1086 1.582.4941zM7.207 13.5273c.4803.3197.5506 1.0577.1563 1.6504-.394.5926-1.1038.8138-1.584.4941-.48-.3197-.5503-1.0577-.1563-1.6504.4008-.6021 1.1087-.8106 1.584-.4941z"/></svg> & WearOS):  Train Around 🏋️‍♂️⌚ 
- workout tracking application
- university project, made in team
- app WearOS + android


### Deep Learning: Road Status Classifier   📊🖼️🛤️
- recognize roads' mantainance statuses
- university project, made in team 
- generation & labelling image dataset
- NN, CNN and transfer learning

### Backend web + Database: MappIt 🗺️📍🍃
- "explorations' social network"
- university project, made in team
- backend Java using Spring framework
- NoSQL technologies as MongoDB and Neo4J

### Internet of Things:  SmartSupermarket 🕸🏭🛒
- university project, made in team 
- IoT network (MQTT & CoAP)
- nodes firmware (Contiki-NG based) 
- server collecting and processing nodes' data 


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
### **Master's Degree:** Artificial Intelligence and Data Engineering
>**University of Pisa**, current


- data mining techniques and algorithms, machine learning and deep learning knowledge
- team work and project management expertise
- design and implementation of distributed systems NoSQL, Android apps and WearOS,  Hadoop and Spark applications
- process management and process mining skills

### Bachelor's Degree: Computer Engineering 
> **University of Pisa**,
> 30 April 2021
>
>Degree mark: 110


- object oriented programming, databases analysis and management skills
- circuits, logical networks, electronics and electrotechnics skills
- cryptanalysis and encryption
- computer networks

## More infos
<details>
  <summary>Interests</summary>
  <p class="topic-badge">artificial intelligence</p>
  <p class="topic-badge">internet of things</p>
  <p class="topic-badge">cloud computing</p>
  <p class="topic-badge">electronics</p>
  <p class="topic-badge">programming</p>
  <p class="topic-badge">DIY</p>
  <p class="topic-badge">web development</p>
  <p class="topic-badge">tech devices</p>
  <p class="topic-badge">drones</p>
  <p class="topic-badge">3D printing</p>
  <p class="topic-badge">CTFs</p>
</details>

<details>
  <summary>Technical knowledge</summary>
  <p class="topic-badge">DBMS MySQL</p>
  <p class="topic-badge">C++</p>
  <p class="topic-badge">JavaScript</p>
  <p class="topic-badge">PHP</p>
  <p class="topic-badge">HTML, CSS</p>
  <p class="topic-badge">Laravel</p>
  <p class="topic-badge">Linux</p>
  <p class="topic-badge">Assembly</p>
  <p class="topic-badge">Python</p>
  <p class="topic-badge">Java</p>
  <p class="topic-badge">MongoDB</p>
  <p class="topic-badge">Neo4J</p>
  <p class="topic-badge">Hadoop</p>
  <p class="topic-badge">Spark</p>
  <p class="topic-badge">TensorFlow</p>
  <p class="topic-badge">Julia</p>
</details>

## Contact Me 📬
Feel free to reach out to me via email at [giacomo@paciosoft.com](mailto:giacomo@paciosoft.com) or connect with me on [LinkedIn](https://dronesimulator.it/r/my-linkedin).