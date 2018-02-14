# DevOps Ramp-up

## Welcome

DevOps has a wide variety of practices, tools, and methodologies, which enable it to be an important part of an _agile delivery culture_.

This ramp-up is presented as a **series of challenges**. Each challenge is chosen to show beginners the basics of some of the DevOps practices, and it is designed to help us use the same language after its completion. We are tool agnostics, so you can use any tool you like, but we do have a client base that need us to be proficient in some basic AWS concepts.



## Challenges


You are going to set up a **Continuous Delivery pipeline** for an application from scratch.

In challenges **1** to **4**, you will have to set up the _Source Code Management tool_ and _branching_ methodologies, set up _cloud based environments_ for the application, gain experience with _configuration management tools_, and set up _Continuous Integration_. All challenges are meant to use the same application.

Challenges **5** to **8** build upon your pipeline to include more practices. These ones are open for you to choose the tool stack of your preference.

---
### **0. Linux Basics**
This is an optional challenge and should be taken if you feel like refreshing your RHEL/GNU Linux knowledge. Just complete [this course](https://app.pluralsight.com/library/courses/lfcs-red-hat-7-essentials/ "LFCS: Linux Essentials").

---
### **1. SCM: Set up git-flow**

The objective of this challenge is to set up [git-flow](http://nvie.com/posts/a-successful-git-branching-model/ "Git-Flow original proposal") on a GitHub repository. 

- Clone these repositories (if you are using Windows, install [Git for Windows](https://git-scm.com/download/win "Git for Windows") in case you haven't already...).

`git clone https://github.com/juan-ruiz/movie-analyst-api.git`

`git clone https://github.com/juan-ruiz/movie-analyst-ui.git`


- Create *n **FIXME*** branches

- Create a branching strategy and provide a diagram of how the git flow works and the commands needed to interact to it for each actor in a software delivery team (developer, design lead, tester).

---
### **2. AWS**

The objective of this challenge is to set up the environments on which the application will run.

To complete this challenge, create the environments to run the application you cloned in the last challenge. There are 2 setups. Create at least the first one to complete the Challenge.


#### SetUp 1

![alt text][logo]

[logo]:https://bitbucket.endava.com/projects/BD/repos/devops-rampup/raw/AWSSetup1.png?at=refs%2Fheads%2Fmaster "First SetUp"

Some of the steps needed:
 - Create an AWS account
 - Setup a custom VPC.
 - Create a public and a private subnet.
 - Create route tables.
 - Setup a connection to internet (Internet Gateway and NAT).
 - Create ACL and SG's (Security).
 - Setup EC2 instances.

#### SetUp 2
In case you already have some knowledge on AWS basics, this setup is meant to create a high availability architecture. This one is optional.


Additional steps for this setup.
  - Setup an Elastic Load Balancer.
  - Create a new subnet in a different availability zone.
  - Set up a DMZ with a proxy server (Nginx is recommended).
  - Use RDS service to create a read replica in one of the AZs.

---
### **3. Configuration Management**

To complete this challenge, use any CM tool to automate the deployment of the application requirements in the newly created environment. See the 2 application folders in order to find out what their dependencies are. Some of the tools we use are Chef, Puppet, and Ansible.

---
### **4. CI/CD**

To complete this challenge, create all the Jenkins jobs needed to automate CI/CD on the newly created environment. Check the application folders, create separate repos and deploy them automatically every time there's a new change in the code repository. If you feel like using a different CI tool, please do!

---
### **5. Monitoring**
To complete this challenge, define a tool stack, install and set up a monitoring strategy for the environments.

---
### **6. Containerization**
To complete this challenge, create registry, dockerfiles and images for the installed apps.

---
### **7. Orchestration and clustering**

To complete this challenge, choose a tool and create cluster for the app we've used.

---
### **8. Infrastructure as code**

To complete this challenge, choose tool and create the necessary scripts to automate the provisioning of the environments for the application.

---
### **9. Showcase challenge**

If you still have time to spare, create your own challenge and show the rest of us the implementation of other DevOps dealings. Examples: Artifact Repository configuration, Test Automation Frameworks integration, Database deployment automation, packaging management automation, build scripting frameworks, release management tools, etc.