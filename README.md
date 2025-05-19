# Visa_approval

Tintu Thomas@TintuThomasVaniyakeriyil MINGW64 /d/GenAI_myworks/Visa_approval (main)
$ git add .

Tintu Thomas@TintuThomasVaniyakeriyil MINGW64 /d/GenAI_myworks/Visa_approval (main)
$ git commit -m "My first commit"
[main 6eae2fb] My first commit
 29 files changed, 50 insertions(+)
 create mode 100644 .dockerignore
 create mode 100644 Dockerfile
 create mode 100644 app.py
 create mode 100644 config/model.yaml
 create mode 100644 config/schema.yaml
 create mode 100644 demo.py
 create mode 100644 requirements.txt
 create mode 100644 setup.py
 create mode 100644 template.py
 create mode 100644 us_visa/__init__.py
 create mode 100644 us_visa/components/__init__.py
 create mode 100644 us_visa/components/data_ingestion.py
 create mode 100644 us_visa/components/data_transformation.py
 create mode 100644 us_visa/components/data_validation.py
 create mode 100644 us_visa/components/model_evaluation.py
 create mode 100644 us_visa/components/model_pusher.py
 create mode 100644 us_visa/components/model_trainer.py
 create mode 100644 us_visa/configuration/__init__.py
 create mode 100644 us_visa/constants/__init__.py
 create mode 100644 us_visa/entity/__init__.py
 create mode 100644 us_visa/entity/artifact_entity.py
 create mode 100644 us_visa/entity/config_entity.py
 create mode 100644 us_visa/exception/__init__.py
 create mode 100644 us_visa/logger/__init__.py
 create mode 100644 us_visa/pipline/__init__.py
 create mode 100644 us_visa/pipline/prediction_pipeline.py
 create mode 100644 us_visa/pipline/training_pipeline.py
 create mode 100644 us_visa/utils/__init__.py
 create mode 100644 us_visa/utils/main_utils.py

Tintu Thomas@TintuThomasVaniyakeriyil MINGW64 /d/GenAI_myworks/Visa_approval (main)
$ git push origin main
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 12 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (11/11), 1.62 KiB | 150.00 KiB/s, done.
Total 11 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/TINTUEEECEC/Visa_approval.git
   cf9bd74..6eae2fb  main -> main

Tintu Thomas@TintuThomasVaniyakeriyil MINGW64 /d/GenAI_myworks/Visa_approval (main)


Anaconda: https://www.anaconda.com/
Vs code: https://code.visualstudio.com/download
Git: https://git-scm.com/
Flowchart: https://whimsical.com/login





Github link: https://github.com/entbappy/US-Visa-Approval-Prediction
Autocomplete tool: Tabnine
MongoDB: https://account.mongodb.com/account/login
Slide: https://docs.google.com/presentation/d/1A_3ne0igLvWSIZqYDFcpT41hkxdj55bDy889Bi9G0ZQ/edit?usp=sharing


# US-Visa-Approval-Prediction

## Live matarials docs

[link](https://docs.google.com/document/d/1UFiHnyKRqgx8Lodsvdzu58LbVjdWHNf-uab2WmhE0A4/edit?usp=sharing)


## Git commands

```bash
git add .

git commit -m "Updated"

git push origin main
```

## How to run?

```bash
conda create -n visa python=3.8 -y
```

```bash
conda activate visa
```

```bash
pip install -r requirements.txt
```

```bash
python app.py
```


## Workflow

1. constant
2. config_entity
3. artifact_entity
4. conponent
5. pipeline
6. app.py / demo.py


### Export the  environment variable
```bash


export MONGODB_URL="mongodb+srv://<username>:<password>...."

export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>

export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>
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
    - Save the URI: 136566696263.dkr.ecr.us-east-1.amazonaws.com/mlproject

	
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

   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_DEFAULT_REGION
   - ECR_REPO

    