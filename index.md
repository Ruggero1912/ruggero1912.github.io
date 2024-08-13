<h1 style="display:flex; justify-content:space-between;"> 
<span style="align-self: flex-end;">👋 Hi! I'm Giacomo Pacini </span>
<img style="border-radius:50%; max-width:100px;" src="{{ '/me.jpeg' | relative_url }}" alt="a picture of me" />
</h1>

<!-- ## About Me ℹ️ -->
<!-- I am a passionate software engineer currently pursuing my Master's degree in Artificial Intelligence and Data Engineering at the University of Pisa, following my Bachelor's degree in Computer Engineering from the same institution. 

With a strong foundation in software engineering, coupled with expertise in deep learning, cloud computing, and data engineering, I am dedicated to leveraging technology to solve complex problems and drive innovation. --->


I am a passionate software engineer freshly graduated in the Master's degree in Artificial Intelligence and Data Engineering at the University of Pisa, following my Bachelor's degree in Computer Engineering from the same institution. <br/>
With a strong foundation in computer engineering, coupled with expertise in deep learning, cloud computing, and data engineering, I am dedicated to leveraging technology to solve complex challenges and drive innovation.

#### My interests

I love designing and developing things that impact on people’s everyday life.
My main skill is **logical thinking**, and I like to apply it to software engineering problems.

#### What I'm doing

I am currently working on my master’s thesis and I am searching for a job opportunity that would make me grow.


## Projects 💻

### dronesimulator 🚁📝🔎
- **Description:** I developed a web platform that simulates the exam needed to achieve the Open Category UAS pilot certificate (drone pilot), it currently has **more than 21.000 users**.<br/>
It *implements* machine *learning techniques* for *questions classification*.
- **Technologies Used:** PHP, SQL, JavaScript, Python, Flask, SciKit-Learn
- **Link:** [dronesimulator.it](https://dronesimulator.it)
- **More details**: [here]({{ '/projects/dronesimulator' | relative_url }})

### TravelTales 🚗♫📰👥
- **Description:** An in-car service that generates a radio feed customized on passengers' interests exploiting various machine learning and AI techniques.
- **Technologies used:** deep neural networks, transformers, dense information retrieval, TTS, face recognition, voice recognition, emotion recognition
- university project, made in team
- the aim of TravelTales is to fuel car conversations by generating personalized news feeds
- exploit emotions to estimate passengers engagement levels
- **More details:** [here]({{ '/projects/traveltales' | relative_url }})

### Mobile (<svg role="img" viewBox="0 0 24 24" width=24 height =24 xmlns="http://www.w3.org/2000/svg"><title>Android</title><path fill="#34A853" d="M18.4395 5.5586c-.675 1.1664-1.352 2.3318-2.0274 3.498-.0366-.0155-.0742-.0286-.1113-.043-1.8249-.6957-3.484-.8-4.42-.787-1.8551.0185-3.3544.4643-4.2597.8203-.084-.1494-1.7526-3.021-2.0215-3.4864a1.1451 1.1451 0 0 0-.1406-.1914c-.3312-.364-.9054-.4859-1.379-.203-.475.282-.7136.9361-.3886 1.5019 1.9466 3.3696-.0966-.2158 1.9473 3.3593.0172.031-.4946.2642-1.3926 1.0177C2.8987 12.176.452 14.772 0 18.9902h24c-.119-1.1108-.3686-2.099-.7461-3.0683-.7438-1.9118-1.8435-3.2928-2.7402-4.1836a12.1048 12.1048 0 0 0-2.1309-1.6875c.6594-1.122 1.312-2.2559 1.9649-3.3848.2077-.3615.1886-.7956-.0079-1.1191a1.1001 1.1001 0 0 0-.8515-.5332c-.5225-.0536-.9392.3128-1.0488.5449zm-.0391 8.461c.3944.5926.324 1.3306-.1563 1.6503-.4799.3197-1.188.0985-1.582-.4941-.3944-.5927-.324-1.3307.1563-1.6504.4727-.315 1.1812-.1086 1.582.4941zM7.207 13.5273c.4803.3197.5506 1.0577.1563 1.6504-.394.5926-1.1038.8138-1.584.4941-.48-.3197-.5503-1.0577-.1563-1.6504.4008-.6021 1.1087-.8106 1.584-.4941z"/></svg> & WearOS):  Train Around 🏋️‍♂️⌚ 
- teams’ workout tracking application: the aim is to control athletes health and training status live
- mobile apps for WearOS (athletes) and for android (trainer)
- creates a Bluetooth Low Energy network of athletes sending real-time training data to a trainer
- **More details:** [here]({{ '/projects/trainaround' | relative_url }})


### Deep Learning: Road Status Classifier   📊🖼️🛤️
- recognize roads' mantainance statuses
- university project, made in team 
- generation & labelling image dataset
- NN, CNN and transfer learning

### Backend web + Database: MappIt 🗺️📍🍃
- "explorations' social network": discover new places to visit and share adventures and experiences
- Java backend implementation using Spring framework
- NoSQL technologies such as MongoDB and Neo4J
- **More details:** [here]({{ '/projects/mappit' | relative_url }})

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
>**University of Pisa**, 
>26th July 2024
>
>Degree mark: 110/110 cum laude

- data mining techniques and algorithms, **machine learning** and **deep learning** knowledge
- **team work and project management** expertise
- design and implementation of distributed systems **NoSQL**
- **Android** and **WearOS** apps development and programming principles
- process management and **process mining** skills
- **cloud computing**: infrastructural models, cloud platforms and cloud programming models (**Hadoop** and **Spark** applications)

### Bachelor's Degree: Computer Engineering 
> **University of Pisa**,
> 30 April 2021
>
>Degree mark: 110/110


- object oriented programming, databases analysis and management skills
- logical networks, computer architectures, digital electronics skills

## More infos
<details>
  <summary>Interests</summary>
  <p class="topic-badge">artificial intelligence</p>
  <p class="topic-badge">drones</p>
  <p class="topic-badge">smart home</p>
  <p class="topic-badge">personal finance</p>
  <p class="topic-badge">cloud computing</p>
  <p class="topic-badge">electronics</p>
  <p class="topic-badge">programming</p>
  <p class="topic-badge">DIY</p>
  <p class="topic-badge">web development</p>
  <p class="topic-badge">tech devices</p>
  <p class="topic-badge">3D printing</p>
  <p class="topic-badge">CTFs</p>
  <p class="topic-badge">mobile development</p>
</details>

<details>
  <summary>Programming languages and frameworks</summary>
  <p class="topic-badge" style="background-color: #f5bc1b;">TensorFlow</p>
  <p class="topic-badge">Sci-Kit Learn</p>
  <p class="topic-badge">Julia</p>
  <p class="topic-badge" style="background-color: #80d1f9;">Hadoop</p>
  <p class="topic-badge" style="background-color: #da6008;">Spark</p>
  <p class="topic-badge" style="background-color: #44ac53;">MongoDB</p>
  <p class="topic-badge" style="background-color: black;">Neo4J</p>
  <p class="topic-badge" style="background-color: #de9208;">SQL</p>
  <p class="topic-badge" style="background-color: #4372a2;">Python</p>
  <p class="topic-badge" style="background-color: #e03725;">Java</p>
  <p class="topic-badge">C++</p>
  <p class="topic-badge">Assembly</p>
  <p class="topic-badge">JavaScript</p>
  <p class="topic-badge">HTML, CSS</p>
  <p class="topic-badge" style="background-color: #556198;">PHP</p>
  <p class="topic-badge" style="background-color: #f33808;">Laravel</p>
</details>

<details>
  <summary>Technical knowledge</summary>
  <p class="topic-badge">OOP</p>
  <p class="topic-badge">cloud models</p>
  <p class="topic-badge">NoSQL</p>
  <p class="topic-badge">IoT</p>
  <p class="topic-badge">Data Mining</p>
  <p class="topic-badge">Machine Learning</p>
  <p class="topic-badge">Deep Learning</p>
  <p class="topic-badge">Reinforcement Learning</p>
  <p class="topic-badge">Evolutionary AI</p>
  <p class="topic-badge">Linux</p>
  <p class="topic-badge">Computer networks</p>
  <p class="topic-badge">Computer architectures</p>
</details>

## Contact Me 📬
Feel free to reach out to me via email at [giacomo@paciosoft.com](mailto:giacomo@paciosoft.com) or connect with me on [LinkedIn](https://dronesimulator.it/r/my-linkedin).