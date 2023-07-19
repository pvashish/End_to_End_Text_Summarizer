# Intelligent Text Summarizer: 📝🔍📜 End-to-End LLM Prompt Engineering Pipeline with GitHub Actions

![Intelligent Text Summarizer](https://github.com/pvashish/End_to_End_Text_Summarizer/blob/main/textS.PNG)

## Project Overview 🚀

Intelligent Text Summarizer is an advanced Natural Language Processing (NLP) project that leverages Hugging Face's transformers library and pre-trained language models to generate accurate text summaries. This end-to-end pipeline is engineered to streamline the process and provide efficient text summarization solutions. With skills in NLP, Transformers - Hugging Face, Docker 🐳, PyTorch 🔥, Pipeline Development - CI/CD 🔄, Git, Python 🐍, and Google Cloud Platform (GCP) ☁️, this project promises cutting-edge technology in the realm of text summarization.

## Key Achievements 🏆

- **Highly Accurate Summarization**: Implemented an end-to-end NLP text summarization pipeline on GCP utilizing Hugging Face's transformers library and pre-trained language models. The system achieved impressive text generation with ROUGE scores up to 0.85, showcasing its precision and reliability. 🎯📈

- **User-Friendly Interface**: Developed a user-friendly interface for the pipeline, significantly reducing processing time for summarizing large documents. This improvement ensures a smooth and accessible experience for users, making the summarization process more efficient and effective. 📚⏱️

- **Efficient Deployment and Scaling**: Leveraged GCP's managed services and Docker for efficient deployment and scaling of the solution. This optimization allows the system to handle large volumes of data seamlessly and ensures high performance even during peak loads. 🚀💨📈

## How to Use 📝🔧

To use the Intelligent Text Summarizer, follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine using the following command:




# End to end Text-Summarizer-Project

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


### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.11 -y
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
Author: Pranavi Vashishtha
Email: v7pranavi@gmail.com

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
    - Save the URI: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

	
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

    AWS_ECR_LOGIN_URI = demo>>  XXXXXXXXXXXXXXXXX

    ECR_REPOSITORY_NAME = simple-app
