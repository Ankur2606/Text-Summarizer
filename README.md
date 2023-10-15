# Text Summarizer

![logo](https://github.com/Ankur2606/Text-Summarizer/assets/66749243/f64420ee-9553-4bf2-a13e-608370eff482)

## Introduction

A sophisticated tool designed to streamline the process of extracting meaningful insights and concise summaries from large volumes of text. In an age where information overload is commonplace, our NLP Summarizer stands as a powerful solution to distill the essence of textual content, saving you time and providing clarity.

The project is driven by state-of-the-art Natural Language Processing (NLP) techniques, making it an invaluable asset for researchers, content creators, or anyone seeking to efficiently condense vast amounts of text while preserving context and accuracy.

It's engineered to excel in precision, flexibility, and ease of integration, serving as a versatile tool for various NLP applications.

## Key Features

Here are some of the key features that set our NLP Summarizer apart:

- **NLP Precision**: Our summarizer utilizes advanced NLP algorithms to ensure that summaries maintain context and relevance.

- **Versatility**: Use our NLP Summarizer as a template for your NLP projects, saving you time and effort in project development.

- **User-Friendly**: With an intuitive interface and comprehensive documentation, even those new to NLP can easily integrate and employ our tool.

## Getting Started

Getting started with our NLP Summarizer is straightforward. Follow these steps to set up and start summarizing:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/nlp-summarizer.git
   
2. cd Text-Summarizer
   <br>
3. pip install -r requirements.txt


## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/entbappy/End-to-end-Text-Summarization
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.8 -y
```

```bash
conda activate summary
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


```bash
Author: Krish Naik
Data Scientist
Email: krishnaik06@gmail.com

```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app
