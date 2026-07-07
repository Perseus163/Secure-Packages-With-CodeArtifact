<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Secure Packages with CodeArtifact

**Project Link:** [View Project](http://nextwork.ai/projects/aws-devops-codeartifact-updated)

**Author:** Abdi Ali  
**Email:** abdiali4453@gmail.com

---

![Image](http://nextwork.ai/serene_violet_happy_lemur/uploads/aws-devops-codeartifact-updated_1d79e699)

---

## Introducing Today's Project!

In this project, I will demonstrate how to Secure Packages with Code Artifact, I'm doing this project to practice and utilize my skills as a Cloud Engineer and being able to secure packages will be a fundamental skill.

### Key tools and concepts

Services I used were CodeArtifact, GitHub, EC2. Key concepts I learnt include on how to deploy packages with CodeArtifact, how to install and run web apps on EC2 and using GitHub

### Project reflection

This project took me approximately 3 hours, The most challenging part was solving errors with Git and the XML file.

This project is part of a series of DevOps projects where I'm building a CI/CD pipeline! 

---

## CodeArtifact Repository

CodeArtifact is an ideal tool to use to manage dependencies as its reliable and can be controlled, it is also more secured as you download packages from it instead from other potentially unsecure sources 

A domain is essentially a folder which stores multiple repositories belonging to your project or organisation for simplicity and security

A CodeArtifact repository can have an upstream repository, which is essentially a backup/redundancy to the main repository.

![Image](http://nextwork.ai/serene_violet_happy_lemur/uploads/aws-devops-codeartifact-updated_n4o5p6q7)

---

## CodeArtifact Security

### Issue

 I ran into an error when retrieving a token ( EC2 Instance must have access to the other AWS services in this case CodeArtifact.)

### Resolution

To resolve the error with my security token i did some troubleshooting in the terminal with some AI assistance.

It's security best practice to use IAM roles due to the principle of least privilege and Zero Trust

---

## The JSON policy attached to my role

The JSON policy I set up grants the EC2 instance the authorization to access the Tokens, endpoints and read rights.

![Image](http://nextwork.ai/serene_violet_happy_lemur/uploads/aws-devops-codeartifact-updated_23rp7q8r9)

---

## Maven and CodeArtifact

### To test the connection between Maven and CodeArtifact, I compiled my web app using settings.xml

The settings.xml file configures Maven to connect with CodeArtifact repository

Compiling means turning human readable code into code machine can understand

![Image](http://nextwork.ai/serene_violet_happy_lemur/uploads/aws-devops-codeartifact-updated_c17eace8)

---

## Verify Connection

After compiling, I checked the project repository and I noticed that it updated the marvin upstream repository aswell

![Image](http://nextwork.ai/serene_violet_happy_lemur/uploads/aws-devops-codeartifact-updated_1d79e699)

---

## Uploading My Own Packages

---

---
