# Notes

## Road-map

<center><img src="./images/Roadmap.png"></center>



## Things to Remeber While Learning 

+ A DevOps engineer considering a move to machine learning, here are some points to consider:

    + #### Start with the basics: 
    
        + Familiarize yourself with ML concepts, such as supervised and unsupervised learning, regression, and classification.
    
    + #### Focus on practical applications: 
        
        + Instead of delving deep into theoretical ML, focus on applying ML to DevOps-related problems, such as predictive maintenance or automated testing.
    
    + #### Develop skills in relevant tools and technologies: 
        
        + Learn popular ML frameworks like TensorFlow, PyTorch, or Scikit-Learn, and familiarize yourself with tools like Jupyter Notebooks or AWS SageMaker.
    
    + #### Network with ML professionals: 
        
        + Attend conferences, join online communities, or participate in meetups to learn from experienced ML practitioners and stay updated on industry trends.
    
<br>

+ By understanding the intersection of machine learning and DevOps, you can leverage the strengths of both fields to drive innovation and improvement in your organization.

## What is MLOps ??

<center><img src="./images/mlops_img.png" width="600px"></center>

<br>

+ MLOps focuses on Machine learning, DevOps, and data engineering, which directs toward the building, deploying, and maintaining Machine learning models in a production environment efficiently. 

+ We can consider MLOps as the process of automating machine learning operations using DevOps techniques.

## Difference between DevOps and MLOps

### Devops:-

+ DevOps facilitates a streamlined software development process for designing, testing, deploying, and monitoring any software application in production.

+ DevOps automates the deployment of software applications to production in just a few minutes to maintain them reliably

+ DevOps empowers various teams to execute their software applications in continuous integration and development mode.

+ DevOps bridge the gap between the development and deployment of application by proving automatic code quality checks, tests, and reliable deployment.


### MLOps:-

+ MLOps facilitates a streamlined ML model development process for feature engineering, model training, model deployment, and monitoring of any ML application.

+ MLOps automates the deployment of ML models in production in a faster way.

+ MLOps empowers data science and IT teams to connect, validate, and manage operations effectively.

+ MLOps bridge the gap between model training and deployment in production by automated model retraining,hyperparameter tuning, model assessment, and computing model drift.

#### NOTE: DevOps and MLOPs both focus on end-to-end process automation.

## MLOps main Tools

+ The main goal of MLOps is to develop and deploy Machine Learning (ML) models efficiently in a production environment. 

+ ML Model development needs lots of experiments like model retraining, hyperparameter tuning, model assessment, model drift, and model deployment. To track all of these things we need specialized tools.

+ Here are some of the most common types of tools used in MLOps:

1. **Track ML Experiments:**

    +  For experimentation purposes, we can use tools such as MLlow, ClearML, Neptune, Weights & Biases, and Comet. 
    
    + MLFlow and ClearML are full machine learning life cycle tools. Weights and Bias tracks and visualize the experiments. Neptune is an experiment tracker and model registry.

2. **Containerization:** 

    + For containerization purposes, we can use tools such as Docker, Kubernetes, and other cloud services such as AKS(Azure Kubernetes Service), GKE(Google Kubernetes Engine), and Amazon EKS. 
    
    + Both Docker and Kubernetes are containerization tools used for automating deployment, scaling, and management of containerized applications.
    
3. **CI/CD Pipeline:** 
    
    + For CI/CD purposes, we can use tools such as Jenkins, CircleCI, and GitLab. Jenkins is an open-source continuous integration and delivery tool. 
    
    + GitLab is a complete platform for version control, issue tracking, code review, and CI/CD. 
    
4. **Monitoring:** 

    + For monitoring purposes, we can use Fiddler and great expectations. Fiddler is a machine learning model monitoring and Great expectations is a data monitoring tool.
    
5. **Workflow Management Tool:** 
    
    + For managing workflows, we can use Airflow and Luigi. Airflow is used for scheduling and managing workflows. Luigi is used for complex data pipelines for batch jobs.


## Define Standards/Principles (Core Idea for MLOps)

<center><img src="./images/flow_dia.png"></center>

### 1. Transition Friction :

+ Use notebooks templates that define common functionality eg. database connection template , fetching data etc.

+ Proper documentation.

### 2. Version control system :

+ Version control system for code, data, environments and artifacts.

### 3. Performance :

+ Leverage distributed computing and containerization tools e.g. Docker, Kubernetes.

### 4. Automation :

+ Build workflows, CI/CD pipelines.

+ MLOps is pipeline centric. Put pipelines in production than putting a model.

### 5. Monitoring :

+ Powerful innovative monitoring tools to monitor data, features, distribution, latency, uptime, Memory utilization etc.

+ Monitorting tools like Prometheus, Grafana

### 6. Continuous Training 

+ Automated retraining of models based on triggers or regular frequency.
