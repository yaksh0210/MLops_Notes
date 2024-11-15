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

<center><img src="./images/Diff.png"></center>


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

<br>



## Who gets Benifited from MLOps

+ **Data Scientists** can now foucs more on research and experimentaion while having the overall visibility of their deployed data.

+ **ML Engineers** gets less resistance from understanding the experiment. Reproductibility is no longer a problem.

+ **Application developers** do not need to change the code every time , the model is changed. Model and application are decoupled from each other.

+ **Risk & Compliance team** gets benifited as MLOps infrastructure allows to steamline the internal processes. Since complete lineage is maintained so auditing process is smooth.

+ **Clients** can make better business decisions when they always have the updated model giving predictions.


## Basic Overview of Maurity Level of model in MLOps Azure

|Level | Description | Highlights | Technology |
|------|-------------|------------|------------| 
0	|No MLOps	|Difficult to manage full machine learning model lifecycle <br><br>The teams are disparate and releases are painful <br><br>Most systems exist as "black boxes," little feedback during/post deployment| Manual builds and deployments<br><br>Manual testing of model and application<br><br>No centralized tracking of model performance<br><br>Training of model is manual|
1	|DevOps but no MLOps |Releases are less painful than No MLOps, but rely on Data Team for every new model<br><br>Still limited feedback on how well a model performs in production<br><br>Difficult to trace/reproduce results | Automated builds<br><br>Automated tests for application code |
2	|Automated Training	|Training environment is fully managed and traceable<br><br>Easy to reproduce model<br><br>Releases are manual, but low friction| Automated model training<br><br>Centralized tracking of model training performance<br><br>Model management |
3	|Automated Model Deployment	|Releases are low friction and automatic<br><br>Full traceability from deployment back to original data<br><br>Entire environment managed: train > test > production| Integrated A/B testing of model performance for deployment<br><br>Automated tests for all code<br><br>Centralized tracking of model training performance|
4	| Full MLOps Automated Operations| Full system automated and easily monitored<br><br>Production systems are providing information on how to improve and, in some cases, automatically improve with new models<br><br>Approaching a zero-downtime system |Automated model training and testing<br><br>Verbose, centralized metrics from deployed model|

---

## Maurity Level 0(ad-hoc)

**Manual Processes:** 

+ No formalized workflows for developing, training, or deploying ML models. Everything is done manually.

**Isolated Workflows:** 

+ Models are built and deployed without standard practices or tools. Typically, work is done on an individual basis.

**Lack of Tracking:** 

+ No formal tools or systems for tracking experiments, versions, or model performance.

**No Automation:**

+ No automated pipelines or scripts; tasks are performed manually.
Level

## Maurity Level 1 (Basic Automation [Devops but no MLops])

**Scripted Workflows:**

+ Basic automation of ML processes using custom scripts (e.g., for training and deploying models).

**Version Control:**

+ Introduction of version control systems (like Git) for managing code and sometimes models.

**Experiment Tracking:**

+ Basic tracking of experiments using simple tools or platforms.

**Basic CI/CD Pipelines:**

+ Initial implementation of CI/CD pipelines, mostly for code, with limited integration for ML models.


## Maurity Level 2: Defined Processes (Automated Training)

**End-to-End Pipelines:**

+ Implementation of structured, end-to-end pipelines for data preparation, model training, and deployment.

**Automated CI/CD:**

+  CI/CD pipelines are established for both code and ML workflows, improving deployment automation.

**Model Registry:**

+ Use of a model registry to manage and version models, improving model governance.

**Basic Monitoring:**

+ Introduction of basic monitoring tools for model performance and operational metrics.

## Maurity Level 3: Managed and Optimized (Automated Training Deployment)

**Integrated Pipelines:**

+ Advanced, automated pipelines with integrated data ingestion, feature engineering, model training, validation, and deployment.

**Continuous Monitoring and Retraining:**

+ Automated monitoring for model performance and data drift, with mechanisms for automated retraining.

**Governance and Compliance:**

+ Implemented policies for model governance, compliance, and auditing.

**Enhanced Collaboration:**

+ Improved collaboration tools and practices, including shared environments and versioned artifacts.

## Maurity Level 4: Scalable and Innovative (Full MLOps Automated Operations)

**Advanced Integration:**

+ Seamless integration of ML workflows with broader DevOps practices and tools for end-to-end management.

**AIOps:**

+ Utilization of AI-driven operations for proactive monitoring, management, and optimization of ML models and infrastructure.

**Adaptive Systems:**

+ Models and systems are adaptive with self-healing capabilities to handle anomalies and optimize performance autonomously.

**Global Scalability:**

+ Solutions are designed for global scalability, with high availability and fault tolerance.

**Advanced Analytics:**

+ In-depth analytics for detailed insights into model performance, business impact, and operational efficiency.


## MLOps Stack

### What is MLOps Stacks?

+ With MLOps Stacks, the entire model development process is implemented, saved, and tracked as code in a source-controlled repository. 

+ Automating the process in this way facilitates more repeatable, predictable, and systematic deployments and makes it possible to integrate with your CI/CD process. 

+ Representing the model development process as code enables you to deploy the code instead of deploying the model. 

+ Deploying the code automates the ability to build the model, making it much easier to retrain the model when necessary.

### How does MLOps Stacks work?

+ When you initiate an MLOps Stacks project, the software steps you through entering the configuration details and then creates a directory containing the files that compose your project. 

+ This directory, or stack, implements the production MLOps workflow recommended by Databricks. 

+ The components shown in the diagram are created for you, and you need only edit the files to add your custom code.

<br>

<center><img src="./images/mlops-stacks-components.png"></center>

<br>


+ In the diagram:

    + A: A data scientist or ML engineer initializes the project using databricks bundle init mlops-stacks. When you initialize the project, you can choose to set up the ML code components (typically used by data scientists), the CI/CD components (typically used by ML engineers), or both.
    
    + B: ML engineers set up Databricks service principal secrets for CI/CD.
    
    + C: Data scientists develop models on Databricks or on their local system.
    
    + D: Data scientists create pull requests to update ML code.
    
    + E: The CI/CD runner runs notebooks, creates jobs, and performs other tasks in the staging and production workspaces.

#### MLOps Stack includes the following three components:


1. **ML code:**

+ MLOps Stacks creates a set of templates for an ML project including notebooks for training, batch inference, and so on. 

+ The standardized template allows data scientists to get started quickly, unifies project structure across teams, and enforces modularized code ready for testing.

2. **ML resources as code:**

+ MLOps Stacks defines resources such as workspaces and pipelines for tasks like training and batch inference. 

+ Resources are defined in Databricks Asset Bundles to facilitate testing, optimization, and version control for the ML environment. 

+ For example, you can try a larger instance type for automated model retraining, and the change is automatically tracked for future reference.

3. **CI/CD:**

+ You can use GitHub Actions or Azure DevOps to test and deploy ML code and resources, ensuring that all production changes are performed through automation and that only tested code is deployed to prod.

<br>

## Architecture Diagram for MLOps 

+ This Architecture shows how to implement continuous integration (CI), continuous delivery (CD), and retraining pipeline for an AI application using Azure DevOps and Azure Machine Learning. 

+ The solution is built on the scikit-learn diabetes dataset but can be easily adapted for any AI scenario and other popular build systems such as Jenkins and Travis.


<center><img src="./images/mlops_architecture.png"></center>


## Architecture Flow

### Train Model

1. Data Scientist writes/updates the code and push it to git repo. This triggers the Azure DevOps build pipeline (continuous integration).

2. Once the Azure DevOps build pipeline is triggered, it runs following types of tasks:

    + Run for new code: Every time new code is committed to the repo, the build pipeline performs data sanity tests and unit tests on the new code.

    + One-time run: These tasks runs only for the first time the build pipeline runs. 
       + It will programatically create an Azure ML Service Workspace, provision Azure ML Compute (used for model training compute), and publish an Azure ML Pipeline. 
       
       + This published Azure ML pipeline is the model training/retraining pipeline.

3. The Azure ML Retraining pipeline is triggered once the Azure DevOps build pipeline completes. 

+ All the tasks in this pipeline runs on Azure ML Compute created earlier. 

+ Following are the tasks in this pipeline:

    + **Train Model** task executes model training script on Azure ML Compute. It outputs a model file which is stored in the run history.
     
    + **Evaluate Model** task evaluates the performance of newly trained model with the model in production. 
        
        + If the new model performs better than the production model, the following steps are executed. 
        
        + If not, they will be skipped.
     
    + **Register Model** task takes the improved model and registers it with the Azure ML Model registry. This allows us to version control it.

### Deploy Model

+ Once you have registered your ML model, you can use Azure ML + Azure DevOps to deploy it.

+ The **Package Model** task packages the new model along with the scoring file and its python dependencies into a docker image and pushes it to Azure Container Registry. 

    + This image is used to deploy the model as web service.

+ The **Deploy Model** task handles deploying your Azure ML model to the cloud (ACI or AKS). 

    + This pipeline deploys the model scoring image into Staging/QA and PROD environments.

+ In the Staging/QA environment, one task creates an Azure Container Instance and deploys the scoring image as a web service on it.

<hr>
<br>

## Which MLOps platform to choose

|Question| Solution|
|--------|-----------|
Do you want managed or unmanaged solution?| **Managed**: Algorithmia , SageMaker, Azure MLOps, Google ML<br><br>**unmanaged**: Kubeflow, Tenserflow,seldon|
What are the data security requirements of your organization? | **Critical data**: On premise solution and you can go with seldon , tenserflow, kubeflow and added on in all these algorithmia has some better features for security<br><br>**non critical data**: Cloud MLOps Solution|
what is complexity of your model??| **Cloud Solution** this are best for scaling like AWS, Azure, Google<br><br>**On-premises** you can go for algorithmia|
Containerization is must|**Custom conatiner**:Kubeflow , Seldon AI<br><br>**Cloud Provider**: Algorithmia, Azure, Google AI, Sagemaker|
CLI vs GUI?| **CLI**: Seldon, Cortex, Optuna<br><br>**GUI** : Kubeflow, Polyaxon etc.|
Which Language and libraries your team is comfartable in?? | **No Java Support**: Polyaxon, Comet, Optuna<br><br>**No Onnx Support**: kubeflow, ployaxon|
What type of machine learning Objective you want to acheive?|**Traditional ML**:Mlflow, Metaflow<br><br>**Deep Learning**:Valhoai, Allegro|
Specialized platform or end-to-end approach??|**Focused** : Algorithmia, Pachyderm<br><br>**End-to-End** : Valohai, Allegro|

## Azure Machine Learning Components

<center><img src="./images/main_components.png"></center>


### Open source tools and Frameworks

<img src="./images/comp1.png">

<br>

+ For model training and inferencing.You can use familiar frameworks like PyTorch, TensorFlow, Scikit-learn, and the new ones being MLflow, Kubeflow, or the open and interoperable ONNX format.

### Data Science Development Tools

<img src="./images/comp2.png">

<br>

+ It simplify your development task.

+ You can choose the one that best meet your needs.From popular IDEs, not limited to Jupyter Notebooks,PyCharm, Visual Code Studio, and CLIs, with programming languages such as Python and R. These are the important ones.

### Automated ML (For those who doesn't like coding or not much familiar with coding)

<img src="./images/comp3.png">

<br>

+ Here there is completely automating the process of creating a model to no code interface for building training and deploying the models of Azure machine learning platform.

+ It has drag-and-drop feature as well as some pre-build modules for generic use cases.

### Entity Management 

<img src="./images/comp4.png">

<br>

+ It allows us to manage different assests used in ML lifecycle like dataset versioning , ML versioning , data profiling to see statistical characteristic of your data sets.

+ It also moinitor drifts in the datasets.


### Security

<img src="./images/comp5.png">

<br>

+ We can access security capabilities such as role-based access , custom machine learning roles, virtual networks and private links.

+ Azure machine learning platform also allows us to get data privacy throughout the machine learning cycle with differential privacy techniques and confidential computing.

## Governance

<img src="./images/comp6.png">

<br>

+ We can also manage governance with policies, audit trails, quotas and cost management.

+ Streamline the complinacne with a comprehansive portfolio spanning 60 certifications including the FedRAMP 5 and DISA IL5 


## Model Serving

<img src="./images/comp7.png">

<br>

+ It has options to deliver models either in batch mode where you have lot of data to score against 

+ you also have option to do real time scoring .

+ for example how to capture credit card fraud transactions.

## Hardware layer 

<img src="./images/comp8.png">

<br>

+ At the hardware layer, we get a powerful Azure infrastructure to accelerate the training and other processes.

+ we also  get to use CPUs, GPUs, DPUs,and FPGA to accelerate deep learning.

+ Also, We can train models on your hybrid infrastructure using Kubernetes cluster on-premises across multi-cloud environments, and at the edge with Azure ARC interoperability.

---

# Building blocks of every MLOps solution

## 1. Training pipeline

<img src="./images/Training_pipeline.png">

**1) Data preparation step:** 
+ It is a set of actions that should extract data from the data source (usually from the data registry), apply processing to prepare data for training, and save the processed version of the data.

**2) Model training step:** 

+ The part of the pipeline that is responsible for the training procedure. As a result of this step, we have model artifacts that include model weights and code for execution. 

+ This list can be extended if needed. 

+ In short words, the output should contain all elements that will be used in inference serving. 

**3) Model evaluation step:** 

+ In some cases, this step can be concatenated with the model training step. 

+ The goal of the evaluation step is to calculate quality metrics from the trained model. 

+ So the output here is quite simple - it is some file with metrics required by the machine learning task.

**4) Model registration step:**

+ The goal of this step is to prepare model artifacts for deployment. 

+ The registration process is specific from one tool to another, and the list of actions performed inside this step is totally different. 

+ The only output should be the same from one solution to another - we should have a new version of the model stored in the model registry.

**5) Deployment step:**

+ It is not a mandatory element for the training pipeline. 

+ Often the model deployment process is a separate step. 

+ But in case it is a part of the training pipeline, it also contains a Condition step that should take a decision about the necessity to deploy the model. 

### How does it work :- 

+ The simplest way is to check the output from the evaluation step. 

+ If the current value is greater than the expected one - green light and let's deploy our model. 

+ The most common approach to deploy a model is to place it on some server with a real-time response that is usually called the endpoint

## 2. Dataset registry

<img src="./images/Dataset_registry.png">

+ data is a core thing of any Data Science solution. Without a good dataset, the training procedure can't guarantee a high quality of the trained model. 

+ That's why selecting the right strategy for storing datasets is crucial for the MLOps solution




#### What is a dataset registry?

+ Physically it can be a database, repository, or any other object storage (depending on the task and preferences of the architect) that should satisfy at least several (not mandatory) points:


    + **Provide API for dataset uploading and downloading:**
        
        + You don't need a tool named dataset registry if you can't operate the data with it.

    + **Provide dataset versioning:** 
    
        + Different runs of the training pipeline can use different versions of the dataset. 
        
        + This information should be stored somehow, and what exactly should be covered by dataset versioning. 
    
    + **Provide API for getting metadata of the dataset:** 
    
        + There are a lot of reasons to store metadata of the dataset. The simplest is just for comparing different versions of the same dataset.


## 3. Model registry

<img src="./images/model_registry.png">

+ The goal of the model registry is similar to the mission of the dataset registry - store trained models and provide all required information about each of them. What should contain the model registry:

    
    + Provide API for model uploading and downloading
    
    + Provide model versioning mechanism
    
    + Metrics storage
    
    + Hyperparameters storage
    
    + Meta information about model artifacts



## 4. Triggering mechanism

<img src="./images/triggering_mechanism.png">


+ MLOps solution should work in automotive mode. 

+ So publishing it once, the developer shouldn't do anything with his pipeline - just make requests to the deployed model. 

+ To achieve this, we need to deal with triggering mechanisms. The idea is quite simple. 

+ The mission of any trigger is waiting for the event described in its requirements. 

+ After the event has occurred, the trigger should start pipeline execution. The simplest example is the dataset update trigger. 

+ It is waiting until a new version of the dataset is created and starting to retrain the model.

## 5. Production pipeline

<img src="./images/production_pipeline.png">

+ A deployment mechanism can be separated from the training pipeline into a block called the production pipeline. 

#### When can it be useful?

+ you don't need to deploy a new model as soon as you train the model with higher accuracy than you have now. 

+ For example, you are waiting for a data structure update, the start of a new month, or any other mysterious triggering event. 

+ Usually, the production pipeline has the following steps inside:

    + Get the best model from the data registry.
    + Deploy new model into endpoint or any other tool.


---

## Extra Topics

## 1. What is canary Deployment??

#### **Canary Deployment:**

+ A deployment strategy that releases a new version of an application or service incrementally to a subset of users, allowing for gradual testing and validation before rolling out to the entire user base.

### **Key Characteristics:**

**Incremental Rollout :** 

+ A small percentage of users are directed to the new version, while the majority remain on the existing version.

**Simultaneous Operation :** 

+ Both the old and new versions run concurrently, allowing for real-time monitoring and testing.

**Gradual Exposure :** 

+ Users are gradually shifted from the old to the new version, enabling detection of potential issues and bugs.

**Rollback Capability :** 

+ If issues arise, the deployment can be quickly rolled back to the previous version, minimizing disruption to users.

### Benefits :

**1. Risk reduction:**

+ Canary deployments reduce the risk of widespread outages or service disruptions by testing the new version with a limited audience.

**2. Faster issue detection:**

+ Problems are identified earlier, allowing for quicker resolution and minimizing downtime.

**3. Improved user experience:**

+ Users are gradually transitioned to the new version, reducing the impact of any issues that may arise.

## 2. what is conda file in mlops

+ In the context of MLOps (Machine Learning Operations), a conda file refers to a package specification file used by conda, a package and environment manager, to install and manage dependencies for a Python project. 

+ A conda file, typically named environment.yml or meta.yaml, describes the dependencies required by your project, including Python packages, libraries, and executables.


+ ```name:``` Specifies the name of the environment.

+ ``dependencies:`` Lists the packages and their versions required by your project.
 
+ ``build:`` Optional section for custom build instructions.
 
+ ``channels:`` Specifies the conda channels (repositories) to search for packages

> Example

```yml
name: mymlproject

dependencies:
  python: 3.9
  scikit-learn: 1.0.2
  pandas: 1.4.4
  numpy: 1.21.2
  torch: 1.12.1
  cudatoolkit: 11.6

build:
  noarch: python

channels:
  - defaults
  - anaconda
```

+ In MLOps, conda files are essential for:
    
    + **Reproducibility:** By specifying exact package versions, you ensure consistent environments across different machines and runs.
    
    + **Dependency management:** Conda files simplify the process of installing and updating dependencies, reducing the risk of version conflicts.
    
    + **Collaboration:** Conda files provide a clear, machine-readable definition of the environment, making it easier for team members to set up and share identical environments.


## 3. MLOps Linting

+ In MLOps, a lint test is a type of automated code review tool that scans machine learning (ML) code for errors, inconsistencies, and best practices.

+ Linting is particularly useful in MLOps to ensure the quality and reliability of ML code, particularly during the development and deployment phases.

### Key Aspects

+ Code Health
+ Code Style
+ Best Practices






+ Made basic overview notes and pushed it to Github

+ And Also complete the course of MLops with azure overview



