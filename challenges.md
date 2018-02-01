# DevOps Ramp-up Projects

Welcome to the Endava Bogotá DevOps Ramp Up site. DevOps has a wide variety of practices, tools and methodologies which enable us to be an important part of and agile delivery culture. Most of the DevOps practitioners are part of the Continuous Delivery Practice. More info on the practice can be found here:

https://conf.endava.com/display/CDP/Continuous+Delivery+Practice

https://weblog.endava.com/continuous-delivery-initiative/introduction-to-cd/

This ramp-up is presented in challenges. Each challenge is chose to show new joiners the basics in some of the DevOps practices, and it is designed to help us use the same language after its completion. We are tool agnostics, so you can use any tool you like, but we do have a client base that need us to be proficient in some basic AWS concepts. They are ordered according our current view of projects necessities.



## Challenges

You are going to set up a Continuous Delivery pipeline for an application from scratch. In challenges 1 to 4, you will have to set up the Source Code Management tool and branching methodologies, set up cloud based environments for the application, gain experience with configuration management tools, and setting up Continuous Integration. All challenges are meant to use the same application.

Challenges 5 to 8 build upon your pipeline to include more practices. These ones are more open for you to choose the tool stack of your preference.


### 0. Linux Basics
This is an optional challenge and should be taken if you feel like refreshing your RHEL knowledge. Just finish this course for completion:
https://www.edx.org/course/fundamentals-red-hat-enterprise-linux-red-hat-rh066x


### 1. SCM: Set up git-flow

The objective of this challenge is to set up git-flow on a bitbucket repository. You will be provided with access to create the branch strategy you need.

 - Clone the repo and create *n FIXME* branches

bash
git clone https://[user]@bitbucket.endava.com/scm/bd/devops-rampup.git

To complete the challenge, create a branching strategy, provide a diagram of how the git flow works and the commands needed to interact to it for each actor in a software delivery team (developer, design lead, tester).


### 2. AWS

The objective of this challenge is to set up the environments on which the application will run.

To complete this challenge, create the environments to run the application you cloned in the last environment.

There are 2 setups. Create at least the first one to complete the Challenge.


#### SetUp 1

![alt text][logo]

[logo]:https://bitbucket.endava.com/projects/BD/repos/devops-rampup/raw/AWSSetup1.png?at=refs%2Fheads%2Fmaster "First SetUp"

Some of the steps needed:
 - Create an AWS account
 - Setup a custom VPC.
 - Create a public and a private VPC.
 - Create route tables.
 - Setup a connection to internet (Internet Gateway and NAT).
 - Create ACL ans SG's (Security).
 - Setup an EC2 instances.

#### SetUp 2
In case you already have some knowledge on AWS basics, this setup is meant to create a high availability architecture. This one is optional.
  ![alt text][logo2]

 [logo2]:https://bitbucket.endava.com/projects/BD/repos/devops-rampup/raw/AWSSetup2.png?at=refs%2Fheads%2Fmaster "First SetUp"

Additional steps for this setup.
  - Setup an Elastic Load Balancer.
  - Create a new subnet in a different availability zone.
  - Set up a DMZ with a proxy server (Nginx is recommended).
  - Use RDS service to create a read replica in one of the AZs.


### 3. Configuration Management

To complete this challenge, use any CM tool to automate the deployment of the application requirements in the newly created environment. See the 2 application folders in order to find out what are their dependencies. Some of the tools we use are Chef, Puppet, and Ansible.

### 4. CI/CD

To complete this challenge, create all the Jenkins jobs needed to automate CI/CD on the newly created environment. Check the application folders create separate repos and deploy them automatically every time there's a new change in the code repository. If you feel like using a different CI tool, please do!


### 5. Monitoring
To complete this challenge, define a tool stack, install and set up a monitoring strategy for the environments.

### 6. Containerization
To complete this challenge, create registry, dockerfiles and images for the installed apps.

### 7. Orchestration and clustering

To complete this challenge, choose a tool and create cluster for the app we've used.

### 8. Infrastructure as a code

To complete this challenge, choose tool and create the necessary scripts to automate the provisioning of the environments for the application.

### 9. Showcase challenge

If you still have time to spare, create your own challenge and show the rest of us the implementation of other DevOps dealings. Examples: Artifact Repository configuration, Test Automation Frameworks integration, Database deployment automation, packaging management automation, build scripting frameworks, release management tools, etc.