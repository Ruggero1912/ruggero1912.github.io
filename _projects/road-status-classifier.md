---
layout: project
name: Road Status Classifier
short_description: Predicting Road Surface Health with Neural Networks and Image Analysis. 
image: /assets/images/roadstatusclassifier/bad-asphalt.png
technologies: Python, TensorFlow, Computer Vision
authors: "Giacomo Pacini, Matteo Pierucci"
date: 2023-06-25
priority: 15
#github: https://github.com/Ruggero1912/
---

RoadHealthNet introduces an innovative approach to assess road surface health using neural networks and image analysis.

### Current Challenges in Road Infrastructure Monitoring

Monitoring road surface health is a critical task for ensuring safety and maintaining high service standards. Traditionally, road inspection relies on manual assessments or expensive specialized equipment. These approaches are often time-consuming, labor-intensive, and difficult to scale over large networks.

Moreover, many road infrastructure companies, such as Anas or Autostrade per l'Italia, face challenges in gathering consistent and actionable data to proactively plan maintenance.

### Characteristics of RoadStatusClassifier

We developed RoadStatusClassifier to address these challenges. Our solution uses a Neural Network Classifier that analyzes images of road surfaces and predicts their health status. A trained model can support the management of road networks by providing real-time feedback about road conditions, which is useful for organizing maintenance actions and ensuring high-quality service.

For instance, a road infrastructure company (e.g., Anas, Autostrade per l'Italia) could periodically collect video footage of roads to be monitored. Frames from the video can be extracted and grouped, and then the Road Status Classifier can automatically estimate the overall health status of a road segment using those frames.

#### Key Features:
- **Real-time Monitoring**: Enables real-time estimation of road surface health using image data.
- **Proactive Maintenance**: Provides actionable insights to schedule maintenance and improve road safety.
- **Flexible Deployment**: Can integrate with existing video surveillance systems or standalone video capturing devices.

#### Technical Innovations:
- Utilizes **transfer learning techniques** and custom datasets to enhance the prediction accuracy of road surface health status.
- Designed with scalability in mind to monitor extensive road networks.


### Technical Approach and Findings

#### Dataset Development

We began by creating an ad-hoc dataset tailored for our classification task. This involved a phase of image scraping followed by a thorough manual revision to ensure data quality and relevance.

#### Neural Network Architectures and Techniques

To identify the best-performing model, we experimented with several pre-trained neural networks, including:
- ResNet50
- VGG16
- MobileNetV2

After extensive testing, ResNet50 emerged as the most suitable architecture for this task, achieving high classification performance, especially for challenging labels like "patched asphalt."

#### Explainability Analysis

Understanding model predictions is critical for trust and practical application. As part of our study, we conducted an in-depth explainability analysis, utilizing techniques such as saliency maps and Grad-CAM to interpret the decisions made by the models.

#### Ensemble Learning with Genetic Algorithms

To further boost performance, we developed an ensemble model using soft-voting. By employing genetic algorithms to optimize the ensemble weights, we achieved the highest recorded classification scores.

### Use Cases

While not designed exclusively for them, infrastructure companies could leverage RoadHealthNet to:
- Automate routine inspections across their networks.
- Reduce costs associated with manual surveys.
- Identify areas needing urgent attention without delay.


<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:7076837221877583872" height="985" width="504" frameborder="0" allowfullscreen="" title="Post incorporato"></iframe>