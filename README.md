# Deploy Artifacts on a Tomcat Server
This configuration ensures that Jenkins automatically triggers a build when code is pushed to GitHub, and the resulting .war file is deployed to your Tomcat server.

![image](https://github.com/user-attachments/assets/0cfc0b54-673b-4c4f-b885-f108723f0e7b)

## Setup CI/CD with GitHub, Jenkins, Maven & Tomcat.
- Setup Jenkins
- Setup & Configure Maven , Git.
- Setup Tomcat Server.
- Integrating GitHub,Maven ,Tomcat Server with Jenkins
- Create a CI and CD Job.
- Test the Deployment.

## Jenkins Stages:
To set up a Jenkins pipeline that performs the following actions:
- **Checkout Code from GitHub**: Automatically triggers when a change is pushed to GitHub.
- **Build with Maven**: Compiles and packages the code.
- **Deploy on Tomcat**: Deploys the resulting .war file to a Tomcat server.

## Prerequisites

### Server Installation
- **Tomcat**: Tomcat should be installed and accessible from Jenkins. You can deploy using SCP, FTP, or direct file copying if Jenkins and Tomcat are on the same server.
- **Jenkins** : Jenkins should be installed and accessible.
- **Maven** : Maven should be installed and accessible from Jenkins

### Jenkins Plugin Installation and Setup
- **Java Setup**: 
![image](https://github.com/user-attachments/assets/9bda1c58-ef34-4442-a4b3-92596e846d4c)

- **GitHub Integration**: Jenkins needs to be configured to trigger builds automatically when a change is pushed to the GitHub repository. This can be done using the GitHub Webhook.
- **Maven Integration**: Maven must be installed and configured in Jenkins.
  ![image](https://github.com/user-attachments/assets/fa6666fc-da5c-44b8-b9ef-d832035ec21b)

- **Credentials**: Credentials for GitHub and Tomcat should be configured in Jenkins.
- **Pipeline: Stage View Plugin**: 
- **Pipeline: Utility Steps Plugin** : it provides the findFiles step.

